FROM microsoft/dotnet:2.2-sdk

MAINTAINER My Name <email@company.com>

ARG http_proxy
ARG https_proxy
ARG no_proxy

ADD Container-Root /

RUN set http_proxy=%http_proxy%; set https_proxy=%https_proxy%; set no_proxy=%no_proxy%; setup.bat; del setup.bat

CMD startup.bat

