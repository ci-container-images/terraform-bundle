FROM golang:1.14
RUN git clone https://github.com/hashicorp/terraform.git -b master && \
    cd terraform/tools && \
    go install ./terraform-bundle/ && \
    mv $GOPATH/bin/terraform-bundle  /bin/ && \
    rm -rf $GOPATH/terraform

CMD ["/bin/bash"]