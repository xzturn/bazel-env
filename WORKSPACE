git_repository(
    name = "jsonnet",
    remote = "https://github.com/google/jsonnet.git",
    tag = "v0.8.1",
)

bind(
    name = "go_prefix",
    actual = "//:go_prefix",
)

new_http_archive(
    name = "golang-linux-amd64",
    build_file = "tools/build_rules/go/toolchain/BUILD.go-toolchain",
    sha256 = "2593132ca490b9ee17509d65ee2cd078441ff544899f6afb97a03d08c25524e7",
    url = "https://storage.googleapis.com/golang/go1.5.1.linux-amd64.tar.gz",
)
