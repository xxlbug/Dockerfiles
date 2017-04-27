FROM alpine:latest

LABEL version="1.0"

# get the necessary tools
RUN apk add --update \
      curl \
      tar

# download prism for linux_amd64
RUN curl https://raw.githubusercontent.com/stoplightio/prism/master/install.sh | sh

# create a new dir for your swagger files
WORKDIR /swagger

# copy all swagger files to the workdir
COPY *.swagger /swagger

# expose the default prism port
EXPOSE 4010

ENTRYPOINT ["prism"]
