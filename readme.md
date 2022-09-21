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
        - [开源防护软件](#开源防护软件)
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

## 资料
- [helm官方文档](https://helm.sh/zh/docs/)
- [k8s包管理工具helm中文文档](https://www.zhaowenyu.com/helm-doc/)

## 蓝队工具

### IAC扫描
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

### IAC用例
- [terraform-examples](https://github.com/futurice/terraform-examples) - Rules based tool to certify Helm charts
- [kubernetes-demo](https://github.com/INT2ECALL/kubernetes-demo) - kubernetes-demo

### 基线检测
- [docker-bench](https://github.com/aquasecurity/docker-bench) - Docker-bench is a Go application that checks whether Docker is deployed securely by running the checks documented in the CIS Docker Benchmark.

### 供应链安全
- [cosign](https://github.com/sigstore/cosign) - Container Signing, Verification and Storage in an OCI registry.
- [DependencyCheck](https://github.com/jeremylong/DependencyCheck) - Dependency-Check is a Software Composition Analysis (SCA) tool that attempts to detect publicly disclosed vulnerabilities contained within a project's dependencies. It does this by determining if there is a Common Platform Enumeration (CPE) identifier for a given dependency. If found, it will generate a report linking to the associated CVE entries.

### 开源防护软件
- [neuvector](https://github.com/neuvector/neuvector) - NeuVector Full Lifecycle Container Security Platform delivers the only cloud-native security with uncompromising end-to-end protection from DevOps vulnerability protection to automated run-time security, and featuring a true Layer 7 container firewall.
- [cilium](https://github.com/cilium/cilium) - Cilium is a networking, observability, and security solution with an eBPF-based dataplane. It provides a simple flat Layer 3 network with the ability to span multiple clusters in either a native routing or overlay mode. It is L7-protocol aware and can enforce network policies on L3-L7 using an identity based security model that is decoupled from network addressing.
- [HummerRisk](https://github.com/HummerRisk/HummerRisk) - 自动化搭建从简单到复杂的脆弱云原生靶机环境
### 红队工具
- [CDK](https://github.com/cdk-team/CDK) - Zero Dependency Container Penetration Toolkit

### 云原生相关工具
- [CDK](https://github.com/cdk-team/CDK) - Zero Dependency Container Penetration Toolkit

### 靶场
- [靶场](https://github.com/Metarget/metarget) - 自动化搭建从简单到复杂的脆弱云原生靶机环境。

# 交流讨论

欢迎关注公众号，一起交流学习。
<p align="center">
    <img src="https://s1.ax1x.com/2022/08/27/vWFPpj.png" alt="vWFPpj.png" border="0" />
</p>

