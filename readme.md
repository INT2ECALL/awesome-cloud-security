<div align="center">
    <h1>云安全系列</h1>
    <p>收集与云安全相关的文章和工具</p>
</div>
<br/>

# 索引

- [文章](#文章)

- [蓝队](#蓝队)
    - [工具](#工具)
        - [IAC扫描](#IAC扫描)
        - [IAC用例](#IAC用例)
        - [基线扫描](#基线扫描)
        - [合规](#合规)
        - [供应链安全](#供应链安全)
        - [流量测防护](#流量测防护)
        - [开源防护软件](#开源防护软件)
        - [公司](#公司)
        
- [红队](#红队)
    - [工具](#工具)


- [交流讨论](#交流讨论)

# 内容

## 文章

- [【云攻防系列】从攻击者视角聊聊K8S集群安全（上）](https://xz.aliyun.com/t/11495)
- [K8s提权之RBAC权限滥用](https://xz.aliyun.com/t/11476)
- [云原生之Kubernetes安全](https://xz.aliyun.com/t/10745)
- [浅谈云安全之K8S](https://www.anquanke.com/post/id/245526)
- [K8S Runtime入侵检测之Falco](https://www.anquanke.com/post/id/247989)
- [浅谈云安全之K8S](https://www.anquanke.com/post/id/179623)
- [RunC TOCTOU逃逸CVE-2021-30465分析](https://www.anquanke.com/post/id/250747)
- [docker 利用特权模式逃逸并拿下主机](https://www.anquanke.com/post/id/272400)
- [【技术分享】利用Dirty Cow实现docker逃逸（附演示视频）](https://www.anquanke.com/post/id/84866)
- [2022云原生安全发展24个洞见](https://www.anquanke.com/post/id/273726)
- [Docker逃逸初探](https://www.anquanke.com/post/id/179623)
- [K8s污点容忍度横向主节点](https://blog.csdn.net/weixin_40418457/article/details/125311021)
- [记录一次平平无奇的云上攻防过程](https://zone.huoxian.cn/d/2557)
- [浅谈Service Mesh体系中的Envoy](https://developer.aliyun.com/article/606655)
- [Envoy原理介绍及线上问题踩坑](https://istio.io/latest/zh/blog/2021/istiomeetups-china-report/IstioMeetupChina-EnvoyPrincipleIntroductionAndOnlineProblemPit.pdf)
- [从零开始的Kubernetes攻防](https://github.com/INT2ECALL/my-re0-k8s-security)
- [自动化挖掘gRPC网络接口漏洞](https://mp.weixin.qq.com/s/WzzCFQBgg7BcVUFWT8npuQ)
- [envoy代理下使用wasm开发WAF](https://www.freebuf.com/articles/web/286857.html)
- [Extending Envoy Proxy - WASM Filter with Golang](https://medium.com/trendyol-tech/extending-envoy-proxy-wasm-filter-with-golang-9080017f28ea)
- [k8s攻防脑图](https://github.com/Bywalks/K8s-Mind-Map)
- [云原生安全攻防 | 使用eBPF逃逸容器技术分析与实践](https://security.tencent.com/index.php/blog/msg/206)
- [从攻击者视角聊聊K8S集群安全](https://xz.aliyun.com/t/11652)
- [Security risk analysis for Kubernetes resources](https://github.com/controlplaneio/kubesec)
- [Secure secret management for Kubernetes (with gpg, Google Cloud KMS and AWS KMS backends)](https://github.com/shyiko/kubesec)
- [node-problem-detector](https://github.com/kubernetes/node-problem-detector)
- [云安全架构连载之三-超大型企业混合云安全架构最佳实践](https://mp.weixin.qq.com/s/xkeNxE99ORtVs9EOv0ellQ)
- [kubescape](https://github.com/kubescape/kubescape)
- [detect-secrets](https://github.com/Yelp/detect-secrets)
- [k8s-unused-secret-detector](https://github.com/dtan4/k8s-unused-secret-detector)
- [trufflehog](https://github.com/trufflesecurity/trufflehog)
- [dockle](https://github.com/goodwithtech/dockle)
- [awesome-k8s-security](https://github.com/magnologan/awesome-k8s-security)
- [rbac-police](https://github.com/PaloAltoNetworks/rbac-police/tree/main/lib)
- [kubesec](https://github.com/controlplaneio/kubesec)
- [kubernetes-secrets](https://www.cloudbees.com/videos/kubernetes-secrets)
- [cloud att&&ck](https://cloudsec.huoxian.cn/)
- [Serverless-Goat](https://github.com/OWASP/Serverless-Goat)
- [rbacr](https://github.com/ZhuriLab/rbacr)
- [owasp-kubernetes-top-ten]([https://github.com/ZhuriLab/rbacr](https://madhuakula.com/kubernetes-goat/docs/owasp-kubernetes-top-ten))
- [k8s-env-injector](https://github.com/hmcts/k8s-env-injector)
- [kubernetes-sidecar-injector](https://github.com/ExpediaGroup/kubernetes-sidecar-injector)
- [vArmor](https://github.com/bytedance/vArmor)
- [badrobot](https://github.com/controlplaneio/badrobot)
- [prowler](https://github.com/prowler-cloud/prowler) 公有云合规检测工具

## 资料
- [helm官方文档](https://helm.sh/zh/docs/)
- [k8s包管理工具helm中文文档](https://www.zhaowenyu.com/helm-doc/)
- [Envoy 中文指南](https://icloudnative.io/envoy-handbook/)

## 蓝队工具

### IAC(Infrastructure-as-Code)扫描
- [chart-verifier](https://github.com/redhat-certification/chart-verifier) - Rules based tool to certify Helm charts
- [terraform](https://github.com/hashicorp/terraform) - Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.
- [trivy](https://github.com/aquasecurity/trivy) - Docker containers vulnerability scan
- [kube-bench](https://github.com/aquasecurity/kube-bench) - kube-bench is a tool that checks whether Kubernetes is deployed securely by running the checks documented in the CIS Kubernetes Benchmark.
- [tfsec](https://github.com/aquasecurity/tfsec) - tfsec uses static analysis of your terraform code to spot potential misconfigurations.
- [Tracee](https://github.com/aquasecurity/Tracee) - Tracee: Runtime Security and Forensics using eBPF
- [kubeconform](https://github.com/INT2ECALL/kubeconform) - Kubeconform is a Kubernetes manifests validation tool. Build it into your CI to validate your Kubernetes configuration!
- [kube-linter](https://github.com/INT2ECALL/kube-linter) - KubeLinter analyzes Kubernetes YAML files and Helm charts, and checks them against a variety of best practices, with a focus on production readiness and security.
- [checkov](https://github.com/bridgecrewio/checkov) - Checkov is a static code analysis tool for infrastructure as code (IaC) and also a software composition analysis (SCA) tool for images and open source packages.
- [helm-opa](https://github.com/eicnix/helm-opa) - This plugin enables you to check your rendered templates files again Open Policy Agent policies to ensure that they match your policies.
- [veinmind](https://github.com/chaitin/veinmind-tools) - 容器安全工具集
- [syft](https://github.com/anchore/syft) - A CLI tool and Go library for generating a Software Bill of Materials (SBOM) from container images and filesystems. Exceptional for vulnerability detection when used with a scanner like Grype.
- [grype](https://github.com/anchore/grype) - A vulnerability scanner for container images and filesystems. Easily install the binary to try it out. Works with Syft, the powerful SBOM (software bill of materials) tool for container images and filesystems.
- [nuclei](https://github.com/projectdiscovery/nuclei) - Fast and customisable vulnerability scanner based on simple YAML based DSL.
- [chart-testing](https://github.com/helm/chart-testing) - ct is the the tool for testing Helm charts. It is meant to be used for linting and testing pull requests. It automatically detects charts changed against the target branch.
- [terratest](https://github.com/gruntwork-io/terratest) - Terratest is a Go library that makes it easier to write automated tests for your infrastructure code. 
- [utrace](https://github.com/Gui774ume/utrace) - UTrace is a tracing utility that leverages eBPF to trace both user space and kernel space functions
- [copacetic](https://github.com/project-copacetic/copacetic) - copa is a CLI tool written in Go and based on buildkit that can be used to directly patch container images given the vulnerability scanning results from popular tools like Trivy.

### IAC用例
- [terraform-examples](https://github.com/futurice/terraform-examples) - Rules based tool to certify Helm charts
- [kubernetes-demo](https://github.com/INT2ECALL/kubernetes-demo) - kubernetes-demo
- [helm-charts-examples](https://github.com/gusakk/helm-charts-examples) - helm-charts-examples

### 规则集
- [defsec](https://github.com/aquasecurity/defsec) - DefSec is a collection of Infrastructure-as-Code rules.

### 基线检测
- [kube-bench](https://github.com/aquasecurity/kube-bench) - kube-bench is a tool that checks whether Kubernetes is deployed securely by running the checks documented in the CIS Kubernetes Benchmark.
- [docker-bench](https://github.com/aquasecurity/docker-bench) - Docker-bench is a Go application that checks whether Docker is deployed securely by running the checks documented in the CIS Docker Benchmark.
- [linux-bench](https://github.com/aquasecurity/linux-bench) - Linux-bench is a Go application that checks whether the Linux operating system is configured securely by running the checks documented in the CIS Distribution Independent Linux Benchmark.

### 供应链安全
- [cosign](https://github.com/sigstore/cosign) - Container Signing, Verification and Storage in an OCI registry.
- [DependencyCheck](https://github.com/jeremylong/DependencyCheck) - Dependency-Check is a Software Composition Analysis (SCA) tool that attempts to detect publicly disclosed vulnerabilities contained within a project's dependencies. It does this by determining if there is a Common Platform Enumeration (CPE) identifier for a given dependency. If found, it will generate a report linking to the associated CVE entries.
- [kubeclarity](https://github.com/openclarity/kubeclarity) - KubeClarity is a tool for detection and management of Software Bill Of Materials (SBOM) and vulnerabilities of container images and filesystems. It scans both runtime K8s clusters and CI/CD pipelines for enhanced software supply chain security.

### WAF
- [tong](https://github.com/zksauren/tong) - 基于envoy代理下的wasm waf插件
- [envoy-filter-log4shell](https://github.com/codexlynx/envoy-filter-log4shell) - Plugable Envoy WebAssembly L7 (HTTP) firewall to prevent log4shell vulnerability injections.
- [proxy-wasm-cpp-sdk](https://github.com/proxy-wasm/proxy-wasm-cpp-sdk) - The SDK has dependencies on specific versions of the C++ WebAssembly toolchain Emscripten (https://emscripten.org) and the protobuf library, therefor use of a Docker image is recommended.
- [coraza-proxy-wasm](https://github.com/corazawaf/coraza-proxy-wasm) - Web Application Firewall WASM filter built on top of Coraza and implementing the proxy-wasm ABI. It can be loaded directly from Envoy or also used as an Istio plugin.
- [gotestwaf](https://github.com/wallarm/gotestwaf) - GoTestWAF is a tool for API and OWASP attack simulation that supports a wide range of API protocols including REST, GraphQL, gRPC, WebSockets, SOAP, XMLRPC, and others.

### 流量代理
- [envoy](https://github.com/envoyproxy/envoy) - ENVOY IS AN OPEN SOURCE EDGE AND SERVICE PROXY, DESIGNED FOR CLOUD-NATIVE APPLICATIONS
- [cn-series-helm](https://github.com/PaloAltoNetworks/cn-series-helm) - This repository contains charts and templates for deploying the Palo Alto Networks CN-series containerized firewall using the Helm Package Manager for Kubernetes

### 开源防护软件
- [neuvector](https://github.com/neuvector/neuvector) - NeuVector Full Lifecycle Container Security Platform delivers the only cloud-native security with uncompromising end-to-end protection from DevOps vulnerability protection to automated run-time security, and featuring a true Layer 7 container firewall.
- [cilium](https://github.com/cilium/cilium) - Cilium is a networking, observability, and security solution with an eBPF-based dataplane. It provides a simple flat Layer 3 network with the ability to span multiple clusters in either a native routing or overlay mode. It is L7-protocol aware and can enforce network policies on L3-L7 using an identity based security model that is decoupled from network addressing.
- [HummerRisk](https://github.com/HummerRisk/HummerRisk) - 检测公有云和云原生安全
- [curiefense](https://github.com/curiefense/curiefense) - Curiefense is a new application security platform, which protects sites, services, and APIs. It extends Envoy proxy to defend against a variety of threats, including SQL and command injection, cross site scripting (XSS), account takeovers (ATOs), application-layer DDoS, remote file inclusion (RFI), API abuse, and more.
- [CloudExplorer-Lite](https://github.com/CloudExplorer-Dev/CloudExplorer-Lite) - 开源轻量级云管平台

### 红队工具
- [shovel](https://github.com/SPuerBRead/shovel) - docker escape
- [CDK](https://github.com/cdk-team/CDK) - Zero Dependency Container Penetration Toolkit
- [k0otkit](https://github.com/Metarget/k0otkit) - k0otkit is a universal post-penetration technique which could be used in penetrations against Kubernetes clusters.
- [kubeletctl](https://github.com/cyberark/kubeletctl) - Kubeletctl is a command line tool that implement kubelet's API.

### 云原生相关工具
- [protobuf](https://github.com/protocolbuffers/protobuf) - Protocol Buffers (a.k.a., protobuf) are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data
- [ko](https://github.com/ko-build/ko) - ko is a simple, fast container image builder for Go applications.
- [func-e](https://func-e.io/) - func-e makes running Envoy® easy

- [oci-seccomp-bpf-hook](https://github.com/containers/oci-seccomp-bpf-hook) - Terratest is a Go library that makes it easier to write automated tests for your infrastructure code. 

### 协议解密
- [pbtk](https://github.com/marin-m/pbtk) - Protobuf is a serialization format developed by Google and used in an increasing number of Android, web, desktop and more applications. It consists of a language for declaring data structures, which is then compiled to code or another kind of structure depending on the target implementation.
- [protobuf_decode](https://github.com/oathupdate/protobuf_decode) - decode the protobuf field value without the proto file.
- [protodec](https://github.com/xiofee/protodec) - util can decode protobuf raw

### 靶场
- [靶场](https://github.com/Metarget/metarget) - 自动化搭建从简单到复杂的脆弱云原生靶机环境。

### 监控
https://pkg.go.dev/k8s.io/utils/inotify#Watcher.AddWatch
### 公司
- [deepfence](https://github.com/deepfence) - deppfence
- [deepfence](https://github.com/deepfence) - wiz
- [deepfence](https://github.com/deepfence) - paloalto prisma
- [deepfence](https://github.com/deepfence) - aqua
- [deepfence](https://github.com/deepfence) - arm


### 漏洞修复
- [copacetic](https://github.com/project-copacetic/copacetic) - copa is a CLI tool written in Go and based on buildkit that can be used to directly patch container images given the vulnerability scanning results from popular tools like Trivy.


# 交流讨论

欢迎关注公众号，一起交流学习。
<p align="center">
    <img src="https://s1.ax1x.com/2022/08/27/vWFPpj.png" alt="vWFPpj.png" border="0" />
</p>

