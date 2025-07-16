FROM cropbox/cropbox:v0.3.52

COPY --chown=${NB_USER} . ${HOME}

RUN JULIA_PROJECT=${HOME} julia -e "using Pkg; Pkg.instantiate(); Pkg.precompile()"
