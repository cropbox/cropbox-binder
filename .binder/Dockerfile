FROM cropbox/cropbox:v0.3.33

COPY --chown=${USER} . ${HOME}

RUN JULIA_PROJECT=${HOME} julia -e "using Pkg; Pkg.instantiate(); Pkg.precompile()"
