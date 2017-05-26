FROM ubuntu:14.04

ENV NCARG_ROOT /usr/local/ncl-6.4.0

RUN apt-get update && apt-get install -y libssh2-1 libfontconfig libxrender1 libgfortran3 libgomp1 librtmp0 libldap-2.4-2 libxext6 wget && wget --content-disposition https://www.earthsystemgrid.org/download/fileDownload.html?logicalFileId=246ab3ec-fa02-11e6-a976-00c0f03d5b7c && mkdir "$NCARG_ROOT" && tar -zxf ncl_ncarg-6.4.0-Debian7.11_64bit_gnu472.tar.gz -C "$NCARG_ROOT" && rm ncl_ncarg-6.4.0-Debian7.11_64bit_gnu472.tar.gz && rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["/usr/local/ncl-6.4.0/bin/ncl"]
CMD []
WORKDIR /ncl
