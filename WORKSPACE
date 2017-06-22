workspace(name = "org_tensorflow_tensorboard")

http_archive(
    name = "io_bazel_rules_closure",
    sha256 = "bc41b80486413aaa551860fc37471dbc0666e1dbb5236fb6177cb83b0c105846",
    strip_prefix = "rules_closure-dec425a4ff3faf09a56c85d082e4eed05d8ce38f",
    urls = [
        "http://mirror.bazel.build/github.com/bazelbuild/rules_closure/archive/dec425a4ff3faf09a56c85d082e4eed05d8ce38f.tar.gz",  # 2017-06-02
        "https://github.com/bazelbuild/rules_closure/archive/dec425a4ff3faf09a56c85d082e4eed05d8ce38f.tar.gz",
    ],
)


load("@io_bazel_rules_closure//closure:defs.bzl", "closure_repositories")

closure_repositories()

http_archive(
    name = "io_bazel_rules_go",
    sha256 = "ef1aa6a368808d3aa18cbe588924f15fb8fac75d80860080355595e75eb9a529",
    strip_prefix = "rules_go-0.4.0",
    urls = [
        "https://github.com/bazelbuild/rules_go/archive/0.4.0.tar.gz",
        "http://bazel-mirror.storage.googleapis.com/github.com/bazelbuild/rules_go/archive/0.4.0.tar.gz",
    ],
)

load("@io_bazel_rules_go//go:def.bzl", "go_repositories")

go_repositories()

http_archive(
    name = "io_bazel_rules_webtesting",
    sha256 = "602bd1fd4e2b756baa636c3815ef6686c111b3e30eab534c0fc84e6c8c9a14c3",
    strip_prefix = "rules_webtesting-b875457028e38511d76e067378dacc1ffcb6c75b",
    urls = [
        "https://github.com/bazelbuild/rules_webtesting/archive/b875457028e38511d76e067378dacc1ffcb6c75b.tar.gz",
        "http://bazel-mirror.storage.googleapis.com/github.com/bazelbuild/rules_webtesting/archive/b875457028e38511d76e067378dacc1ffcb6c75b.tar.gz",
    ],
)

http_file(
    name = "org_chromium_chromedriver_linux",
    sha256 = "0c01b05276da98f203dc7eb4236c2ee7fe799b432734e088549bd0aadc71958e",
    url = "http://chromedriver.storage.googleapis.com/2.24/chromedriver_linux64.zip",
)

load("@io_bazel_rules_webtesting//web:repositories.bzl", "web_test_repositories")

web_test_repositories()

load("//third_party:workspace.bzl", "tensorboard_workspace")

# Please add all new dependencies in workspace.bzl.
tensorboard_workspace()
