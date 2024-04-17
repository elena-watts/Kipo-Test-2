FROM rocker/binder:4.3.3
LABEL maintainer='Elena Watts'
COPY --chown=${NB_USER} . ${HOME}
USER ${NB_USER}



RUN wget https://github.com/elena-watts/Kipo-Test-2/raw/master/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2024-04-17/')); devtools::install_deps()"

RUN rm DESCRIPTION.1; exit 0
