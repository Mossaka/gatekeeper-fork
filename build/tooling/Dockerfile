FROM golang:1.24.4-bookworm@sha256:2ba8aa7693241f09f3b6e5526a00234f59ee950e22f0a6b39f8b5cd467895f93

RUN GO111MODULE=on go install sigs.k8s.io/controller-tools/cmd/controller-gen@v0.14.0
RUN GO111MODULE=on go install k8s.io/code-generator/cmd/conversion-gen@v0.29.3

RUN mkdir /gatekeeper
WORKDIR /gatekeeper
