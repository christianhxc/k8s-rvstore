package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "cleanup.go",
        "create.go",
        "exec_util.go",
        "flake_reporting_util.go",
        "framework.go",
        "get-kubemark-resource-usage.go",
        "google_compute.go",
        "kubelet_stats.go",
        "log_size_monitoring.go",
        "metrics_util.go",
        "networking_utils.go",
        "nodes_util.go",
        "perf_util.go",
        "pods.go",
        "profile_gatherer.go",
        "provider.go",
        "psp_util.go",
        "pv_util.go",
        "rc_util.go",
        "resource_usage_gatherer.go",
        "service_util.go",
        "size.go",
        "statefulset_utils.go",
        "test_context.go",
        "util.go",
    ],
    importpath = "k8s.io/kubernetes/test/e2e/framework",
    deps = [
        "//pkg/api/v1/pod:go_default_library",
        "//pkg/apis/apps:go_default_library",
        "//pkg/apis/batch:go_default_library",
        "//pkg/apis/core:go_default_library",
        "//pkg/apis/extensions:go_default_library",
        "//pkg/apis/storage/v1/util:go_default_library",
        "//pkg/client/conditions:go_default_library",
        "//pkg/controller:go_default_library",
        "//pkg/controller/nodelifecycle:go_default_library",
        "//pkg/controller/service:go_default_library",
        "//pkg/features:go_default_library",
        "//pkg/kubelet/apis/config:go_default_library",
        "//pkg/kubelet/apis/stats/v1alpha1:go_default_library",
        "//pkg/kubelet/dockershim/metrics:go_default_library",
        "//pkg/kubelet/events:go_default_library",
        "//pkg/kubelet/metrics:go_default_library",
        "//pkg/kubelet/pod:go_default_library",
        "//pkg/kubelet/sysctl:go_default_library",
        "//pkg/kubelet/util/format:go_default_library",
        "//pkg/master/ports:go_default_library",
        "//pkg/registry/core/service/portallocator:go_default_library",
        "//pkg/scheduler/algorithm/predicates:go_default_library",
        "//pkg/scheduler/metrics:go_default_library",
        "//pkg/scheduler/nodeinfo:go_default_library",
        "//pkg/security/podsecuritypolicy/seccomp:go_default_library",
        "//pkg/util/system:go_default_library",
        "//pkg/util/taints:go_default_library",
        "//pkg/volume/util:go_default_library",
        "//staging/src/k8s.io/api/apps/v1:go_default_library",
        "//staging/src/k8s.io/api/apps/v1beta2:go_default_library",
        "//staging/src/k8s.io/api/batch/v1:go_default_library",
        "//staging/src/k8s.io/api/core/v1:go_default_library",
        "//staging/src/k8s.io/api/extensions/v1beta1:go_default_library",
        "//staging/src/k8s.io/api/policy/v1beta1:go_default_library",
        "//staging/src/k8s.io/api/rbac/v1:go_default_library",
        "//staging/src/k8s.io/api/rbac/v1beta1:go_default_library",
        "//staging/src/k8s.io/api/storage/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/fields:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/types:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/intstr:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/net:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/rand:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/uuid:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/version:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/yaml:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//staging/src/k8s.io/apiserver/pkg/authentication/serviceaccount:go_default_library",
        "//staging/src/k8s.io/apiserver/pkg/util/feature:go_default_library",
        "//staging/src/k8s.io/client-go/discovery:go_default_library",
        "//staging/src/k8s.io/client-go/discovery/cached/memory:go_default_library",
        "//staging/src/k8s.io/client-go/dynamic:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes/scheme:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes/typed/core/v1:go_default_library",
        "//staging/src/k8s.io/client-go/rest:go_default_library",
        "//staging/src/k8s.io/client-go/restmapper:go_default_library",
        "//staging/src/k8s.io/client-go/scale:go_default_library",
        "//staging/src/k8s.io/client-go/tools/cache:go_default_library",
        "//staging/src/k8s.io/client-go/tools/clientcmd:go_default_library",
        "//staging/src/k8s.io/client-go/tools/clientcmd/api:go_default_library",
        "//staging/src/k8s.io/client-go/tools/remotecommand:go_default_library",
        "//staging/src/k8s.io/client-go/tools/watch:go_default_library",
        "//staging/src/k8s.io/client-go/util/retry:go_default_library",
        "//staging/src/k8s.io/component-base/cli/flag:go_default_library",
        "//test/e2e/framework/auth:go_default_library",
        "//test/e2e/framework/ginkgowrapper:go_default_library",
        "//test/e2e/framework/log:go_default_library",
        "//test/e2e/framework/metrics:go_default_library",
        "//test/e2e/framework/ssh:go_default_library",
        "//test/e2e/framework/testfiles:go_default_library",
        "//test/e2e/manifest:go_default_library",
        "//test/e2e/perftype:go_default_library",
        "//test/utils:go_default_library",
        "//test/utils/image:go_default_library",
        "//vendor/github.com/onsi/ginkgo:go_default_library",
        "//vendor/github.com/onsi/ginkgo/config:go_default_library",
        "//vendor/github.com/onsi/gomega:go_default_library",
        "//vendor/github.com/onsi/gomega/types:go_default_library",
        "//vendor/github.com/pkg/errors:go_default_library",
        "//vendor/github.com/prometheus/common/expfmt:go_default_library",
        "//vendor/github.com/prometheus/common/model:go_default_library",
        "//vendor/golang.org/x/net/websocket:go_default_library",
        "//vendor/k8s.io/klog:go_default_library",
        "//vendor/k8s.io/utils/exec:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//test/e2e/framework/auth:all-srcs",
        "//test/e2e/framework/config:all-srcs",
        "//test/e2e/framework/deployment:all-srcs",
        "//test/e2e/framework/endpoints:all-srcs",
        "//test/e2e/framework/ginkgowrapper:all-srcs",
        "//test/e2e/framework/gpu:all-srcs",
        "//test/e2e/framework/ingress:all-srcs",
        "//test/e2e/framework/job:all-srcs",
        "//test/e2e/framework/lifecycle:all-srcs",
        "//test/e2e/framework/log:all-srcs",
        "//test/e2e/framework/metrics:all-srcs",
        "//test/e2e/framework/podlogs:all-srcs",
        "//test/e2e/framework/providers/aws:all-srcs",
        "//test/e2e/framework/providers/azure:all-srcs",
        "//test/e2e/framework/providers/gce:all-srcs",
        "//test/e2e/framework/providers/kubemark:all-srcs",
        "//test/e2e/framework/providers/openstack:all-srcs",
        "//test/e2e/framework/providers/vsphere:all-srcs",
        "//test/e2e/framework/replicaset:all-srcs",
        "//test/e2e/framework/ssh:all-srcs",
        "//test/e2e/framework/testfiles:all-srcs",
        "//test/e2e/framework/timer:all-srcs",
        "//test/e2e/framework/viperconfig:all-srcs",
        "//test/e2e/framework/volume:all-srcs",
    ],
    tags = ["automanaged"],
)
