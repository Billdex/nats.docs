# Table of contents

- [Welcome](../welcome.md)

## 版本说明

- [新功能](../release_notes/whats_new.md)
  - [NATS 2.2](../release_notes/whats_new_22.md)
  - [NATS 2.0](../release_notes/whats_new_20.md)

## NATS 概念

- [概述](../overview.md)
  - [NATS 对比](../nats-concepts/overview/compare-nats.md)
- [什么是 NATS](../nats-concepts/what-is-nats/readme.md)
  - [安装演示](../nats-concepts/what-is-nats/walkthrough_setup.md)
- [主题式消息](../nats-concepts/subjects.md)
- [Core NATS](../nats-concepts/core-nats/readme.md)
  - [发布-订阅模式](../nats-concepts/core-nats/publish-subscribe/pubsub.md)
    - [发布/订阅演示](../nats-concepts/core-nats/publish-subscribe/pubsub_walkthrough.md)
  - [请求-响应模式](../nats-concepts/core-nats/request-reply/reqreply.md)
    - [请求-响应演示](../nats-concepts/core-nats/request-reply/reqreply_walkthrough.md)
  - [队列组](../nats-concepts/core-nats/queue-groups/queue.md)
    - [队列演示](../nats-concepts/core-nats/queue-groups/queues_walkthrough.md)
- [JetStream](../nats-concepts/jetstream/readme.md)
  - [流](../nats-concepts/jetstream/streams.md)
  - [消费者](../nats-concepts/jetstream/consumers.md)
    - [示例](../nats-concepts/jetstream/example_configuration.md)
  - [JetStream 演示](../nats-concepts/jetstream/js_walkthrough.md)
  - [键值存储 Key/Value Store](../nats-concepts/jetstream/key-value-store/readme.md)
    - [键值存储演示](../nats-concepts/jetstream/key-value-store/kv_walkthrough.md)
  - [对象存储 Object Store](../nats-concepts/jetstream/object-store/obj_store.md)
    - [对象存储演示](../nats-concepts/jetstream/object-store/obj_walkthrough.md)
- [主题映射与分区](../nats-concepts/subject_mapping.md)
- [NATS 服务基础设施](../nats-concepts/service_infrastructure.md)
  - [自适应部署体系结构](../nats-concepts/adaptive_edge_deployment.md)
- [安全性](../nats-concepts/security.md)
- [连接性](../nats-concepts/connectivity.md)

## 使用 NATS

- [NATS 工具集](../using-nats/nats-tools/readme.md)
  - [nats](../using-nats/nats-tools/nats_cli/readme.md)
    - [nats bench](../using-nats/nats-tools/nats_cli/natsbench.md)
  - [nk](../using-nats/nats-tools/nk.md)
  - [nsc](../using-nats/nats-tools/nsc/README.md)
    - [基础知识](../using-nats/nats-tools/nsc/basics.md)
    - [Streams](../using-nats/nats-tools/nsc/streams.md)
    - [服务](../using-nats/nats-tools/nsc/services.md)
    - [签名密钥](../using-nats/nats-tools/nsc/signing_keys.md)
    - [撤销](../using-nats/nats-tools/nsc/revocation.md)
    - [管理 Operators](../using-nats/nats-tools/nsc/managed.md)
  - [nats-top](../using-nats/nats-tools/nats_top/README.md)
    - [教程](../using-nats/nats-tools/nats_top/nats-top-tutorial.md)
- [使用 NATS 开发](../using-nats/developing-with-nats/developer.md)
  - [NATS 应用剖析](../using-nats/developing-with-nats/anatomy.md)
  - [连接](../using-nats/developing-with-nats/connecting/README.md)
    - [连接到默认服务](../using-nats/developing-with-nats/connecting/default_server.md)
    - [连接到特定服务](../using-nats/developing-with-nats/connecting/specific_server.md)
    - [连接到集群](../using-nats/developing-with-nats/connecting/cluster.md)
    - [连接名](../using-nats/developing-with-nats/connecting/name.md)
    - [使用用户名和密码鉴权](../using-nats/developing-with-nats/connecting/security/userpass.md)
    - [使用 Token 鉴权](../using-nats/developing-with-nats/connecting/security/token.md)
    - [使用 NKey 鉴权](../using-nats/developing-with-nats/connecting/security/nkey.md)
    - [使用证书文件鉴权](../using-nats/developing-with-nats/connecting/security/creds.md)
    - [使用 TLS 加密连接](../using-nats/developing-with-nats/connecting/security/tls.md)
    - [设置连接超时](../using-nats/developing-with-nats/connecting/connect_timeout.md)
    - [Ping/Pong 协议](../using-nats/developing-with-nats/connecting/pingpong.md)
    - [关闭消息回显](../using-nats/developing-with-nats/connecting/noecho.md)
    - [杂项功能](../using-nats/developing-with-nats/connecting/misc.md)
    - [自动重连](../using-nats/developing-with-nats/reconnect/README.md)
      - [禁用重连](../using-nats/developing-with-nats/reconnect/disable.md)
      - [设置重连尝试次数](../using-nats/developing-with-nats/reconnect/max.md)
      - [避免惊群效应](../using-nats/developing-with-nats/reconnect/random.md)
      - [重连之间的暂停](../using-nats/developing-with-nats/reconnect/wait.md)
      - [监听重连事件](../using-nats/developing-with-nats/reconnect/events.md)
      - [重连期间的消息缓冲](../using-nats/developing-with-nats/reconnect/buffer.md)
    - [监控连接](../using-nats/developing-with-nats/events/README.md)
      - [监听连接事件](../using-nats/developing-with-nats/events/events.md)
      - [慢消费者](../using-nats/developing-with-nats/events/slow.md)
  - [接收消息](../using-nats/developing-with-nats/receiving/README.md)
    - [同步订阅](../using-nats/developing-with-nats/receiving/sync.md)
    - [异步订阅](../using-nats/developing-with-nats/receiving/async.md)
    - [退订](../using-nats/developing-with-nats/receiving/unsubscribing.md)
    - [N 条消息后退订](../using-nats/developing-with-nats/receiving/unsub_after.md)
    - [回复消息](../using-nats/developing-with-nats/receiving/reply.md)
    - [通配符订阅](../using-nats/developing-with-nats/receiving/wildcards.md)
    - [队列订阅](../using-nats/developing-with-nats/receiving/queues.md)
    - [断开连接前清除消息](../using-nats/developing-with-nats/receiving/drain.md)
    - [接收结构化数据](../using-nats/developing-with-nats/receiving/structure.md)
  - [发送消息](../using-nats/developing-with-nats/sending/README.md)
    - [包含回复主题](../using-nats/developing-with-nats/sending/replyto.md)
    - [请求-响应语义](../using-nats/developing-with-nats/sending/request_reply.md)
    - [缓存, 刷新 和 Ping](../using-nats/developing-with-nats/sending/caches.md)
    - [发送结构化数据](../using-nats/developing-with-nats/sending/structure.md)
  - [JetStream](../using-nats/jetstream/develop_jetstream.md)
    - [深入探索 JetStream 模型](../using-nats/jetstream/model_deep_dive.md)
    - [管理流和消费者](../using-nats/developing-with-nats/js/streams.md)
    - [发布到流](../using-nats/developing-with-nats/js/publish.md)
    - [使用键值存储](../using-nats/developing-with-nats/js/kv.md)
    - [使用对象存储](../using-nats/developing-with-nats/js/object.md)
  - [教程](../using-nats/developing-with-nats/tutorials/README.md)
    - [Go 中的高级连接与自定义拨号](../using-nats/developing-with-nats/tutorials/custom_dialer.md)

## 运行 NATS 服务

- [安装、运行和部署 NATS 服务](../running-a-nats-service/introduction.md)
  - [安装 NATS 服务](../running-a-nats-service/installation.md)
  - [运行和部署 NATS 服务](../running-a-nats-service/running/README.md)
  - [Windows Service](../running-a-nats-service/running/windows_srv.md)
  - [Flags](../running-a-nats-service/running/flags.md)
- [NATS 和 Docker](../running-a-nats-service/running/nats_docker/README.md)
  - [教程](../running-a-nats-service/running/nats_docker/nats-docker-tutorial.md)
  - [Docker Swarm](../running-a-nats-service/running/nats_docker/docker_swarm.md)
  - [在 Docker 中运行 Python 和 NGS](../running-a-nats-service/running/nats_docker/ngs-docker-python.md)
  - [JetStream](../running-a-nats-service/running/nats_docker/jetstream_docker.md)
- [NATS 和 Kubernetes](../running-a-nats-service/nats-on-kubernetes/nats-kubernetes.md)
  - [使用 Helm 部署 NATS](../running-a-nats-service/nats-on-kubernetes/helm-charts.md)
  - [创建 Kubernetes 集群](../running-a-nats-service/nats-on-kubernetes/create-k8s-cluster.md)
  - [NATS 集群和证书管理](../running-a-nats-service/nats-on-kubernetes/nats-cluster-and-cert-manager.md)
  - [使用 cfssl 证书保护 NATS 集群](../running-a-nats-service/nats-on-kubernetes/operator-tls-setup-with-cfssl.md)
  - [为外部访问 NATS 配置负载均衡](../running-a-nats-service/nats-on-kubernetes/nats-external-nlb.md)
  - [使用 Helm 在 Digital Ocean 上创建 NATS 超级集群](../running-a-nats-service/nats-on-kubernetes/super-cluster-on-digital-ocean.md)
  - [使用 Helm 从零到 K8S 再到 Leafnodes](../running-a-nats-service/nats-on-kubernetes/from-zero-to-leafnodes.md)
- [NATS 服务客户端](../running-a-nats-service/clients.md)
- [配置 NATS 服务](../running-a-nats-service/configuration/README.md)
  - [配置 JetStream](../running-a-nats-service/configuration/jetstream-config/resource_management.md)
    - [配置管理](../running-a-nats-service/configuration/jetstream-config/configuration_mgmt/README.md)
      - [NATS Admin CLI](../running-a-nats-service/configuration/jetstream-config/configuration_mgmt/nats-admin-cli.md)
      - [Terraform](../running-a-nats-service/configuration/jetstream-config/configuration_mgmt/terraform.md)
      - [GitHub Actions](../running-a-nats-service/configuration/jetstream-config/configuration_mgmt/github_actions.md)
      - [Kubernetes Controller](../running-a-nats-service/configuration/jetstream-config/configuration_mgmt/kubernetes_controller.md)
  - [集群](../running-a-nats-service/configuration/clustering/README.md)
    - [集群配置](../running-a-nats-service/configuration/clustering/cluster_config.md)
    - [JetStream 集群](../running-a-nats-service/configuration/clustering/jetstream_clustering/README.md)
      - [管理](../running-a-nats-service/configuration/clustering/jetstream_clustering/administration.md)
  - [带网关的超级集群](../running-a-nats-service/configuration/gateways/README.md)
    - [配置](../running-a-nats-service/configuration/gateways/gateway.md)
  - [Leaf Nodes](../running-a-nats-service/configuration/leafnodes/README.md)
    - [配置](../running-a-nats-service/configuration/leafnodes/leafnode_conf.md)
    - [JetStream on Leaf Nodes](../running-a-nats-service/configuration/leafnodes/jetstream_leafnodes.md)
  - [NATS 安全](../running-a-nats-service/configuration/securing_nats/README.md)
    - [启用 TLS](../running-a-nats-service/configuration/securing_nats/tls.md)
    - [身份验证](../running-a-nats-service/configuration/securing_nats/auth_intro/README.md)
      - [Tokens](../running-a-nats-service/configuration/securing_nats/auth_intro/tokens.md)
      - [用户名/密码](../running-a-nats-service/configuration/securing_nats/auth_intro/username_password.md)
      - [TLS 验证](../running-a-nats-service/configuration/securing_nats/auth_intro/tls_mutual_auth.md)
        - [集群中的 TLS 验证](../running-a-nats-service/configuration/clustering/cluster_tls.md)
      - [NKeys](../running-a-nats-service/configuration/securing_nats/auth_intro/nkey_auth.md)
      - [鉴权超时](../running-a-nats-service/configuration/securing_nats/auth_intro/auth_timeout.md)
      - [去中心化的 JWT 认证/授权](../running-a-nats-service/configuration/securing_nats/jwt/README.md)
        - [使用解析器检查账户](../running-a-nats-service/configuration/securing_nats/jwt/resolver.md)
        - [内存解析器教程](../running-a-nats-service/configuration/securing_nats/jwt/mem_resolver.md)
        - [混合认证/授权设置](../running-a-nats-service/configuration/securing_nats/jwt/jwt_nkey_auth.md)
    - [授权](../running-a-nats-service/configuration/securing_nats/authorization.md)
    - [使用帐户的多租户](../running-a-nats-service/configuration/securing_nats/accounts.md)
    - [装订 OCSP](../running-a-nats-service/configuration/ocsp.md)
  - [日志](../running-a-nats-service/configuration/logging.md)
  - [启用监控](../running-a-nats-service/configuration/monitoring.md)
  - [MQTT](../running-a-nats-service/configuration/mqtt/README.md)
    - [配置](../running-a-nats-service/configuration/mqtt/mqtt_config.md)
  - [配置主题映射](../running-a-nats-service/configuration/configuring_subject_mapping.md)
  - [系统事件](../running-a-nats-service/configuration/sys_accounts/README.md)
    - [系统事件与去中心化 JWT 教程](../running-a-nats-service/configuration/sys_accounts/sys_accounts.md)
  - [WebSocket](../running-a-nats-service/configuration/websocket/README.md)
    - [配置](../running-a-nats-service/configuration/websocket/websocket_conf.md)
- [管理和监控 NATS 服务基础设施](../running-a-nats-service/nats_admin/README.md)
  - [监控](../running-a-nats-service/nats_admin/monitoring/readme.md)
    - [监控 JetStream](../running-a-nats-service/nats_admin/monitoring/monitoring_jetstream.md)
  - [管理 JetStream](../running-a-nats-service/nats_admin/jetstream_admin/README.md)
    - [账户信息](../running-a-nats-service/nats_admin/jetstream_admin/account.md)
    - [命名 Streams, Consumers 与 Accounts](../running-a-nats-service/nats_admin/jetstream_admin/naming.md)
    - [Streams](../running-a-nats-service/nats_admin/jetstream_admin/streams.md)
    - [消费者](../running-a-nats-service/nats_admin/jetstream_admin/consumers.md)
    - [数据复制](../running-a-nats-service/nats_admin/jetstream_admin/replication.md)
    - [灾难恢复](../running-a-nats-service/nats_admin/jetstream_admin/disaster_recovery.md)
    - [静态加密](../running-a-nats-service/nats_admin/jetstream_admin/encryption_at_rest.md)
  - [管理 NATS 安全](../running-a-nats-service/nats_admin/security.md)
    - [深度 JWT 指南](../running-a-nats-service/nats_admin/jwt.md)
  - [升级集群](../running-a-nats-service/nats_admin/upgrading_cluster.md)
  - [慢消费者](../running-a-nats-service/nats_admin/slow_consumers.md)
  - [信号](../running-a-nats-service/nats_admin/signals.md)
  - [跛鸭模式](../running-a-nats-service/nats_admin/lame_duck_mode.md)

## 参考

- [FAQ](../reference/faq.md)
- [NATS 协议](../reference-protocols.md)
  - [协议 Demo](../reference/nats-protocol/nats-protocol-demo.md)
  - [客户端协议](../reference/nats-protocol/nats-protocol/README.md)
    - [开发客户端](../reference/nats-protocol/nats-protocol/nats-client-dev.md)
  - [NATS 集群协议](../reference/nats-protocol/nats-server-protocol.md)
  - [JetStream wire API 参考](../using-nats/jetstream/nats_api_reference.md)

## 遗留文档

- [STAN aka 'NATS Streaming'](../legacy/stan/README.md)
  - [STAN Concepts](../legacy/stan/nats-streaming-concepts/intro.md)
    - [Relation to NATS](../legacy/stan/nats-streaming-concepts/relation-to-nats.md)
    - [Client Connections](../legacy/stan/nats-streaming-concepts/client-connections.md)
    - [Channels](../legacy/stan/nats-streaming-concepts/channels/README.md)
      - [Message Log](../legacy/stan/nats-streaming-concepts/channels/message-log.md)
      - [Subscriptions](../legacy/stan/nats-streaming-concepts/channels/subscriptions/README.md)
        - [Regular](../legacy/stan/nats-streaming-concepts/channels/subscriptions/regular.md)
        - [Durable](../legacy/stan/nats-streaming-concepts/channels/subscriptions/durable.md)
        - [Queue Group](../legacy/stan/nats-streaming-concepts/channels/subscriptions/queue-group.md)
        - [Redelivery](../legacy/stan/nats-streaming-concepts/channels/subscriptions/redelivery.md)
    - [Store Interface](../legacy/stan/nats-streaming-concepts/store-interface.md)
    - [Store Encryption](../legacy/stan/nats-streaming-concepts/store-encryption.md)
    - [Clustering](../legacy/stan/nats-streaming-concepts/clustering/README.md)
      - [Supported Stores](../legacy/stan/nats-streaming-concepts/clustering/supported-stores.md)
      - [Configuration](../legacy/stan/nats-streaming-concepts/clustering/configuration.md)
      - [Auto Configuration](../legacy/stan/nats-streaming-concepts/clustering/auto-configuration.md)
      - [Containers](../legacy/stan/nats-streaming-concepts/clustering/containers.md)
    - [Fault Tolerance](../legacy/stan/nats-streaming-concepts/ft/README.md)
      - [Active Server](../legacy/stan/nats-streaming-concepts/ft/active-server.md)
      - [Standby Servers](../legacy/stan/nats-streaming-concepts/ft/standby-server.md)
      - [Shared State](../legacy/stan/nats-streaming-concepts/ft/shared-state.md)
      - [Failover](../legacy/stan/nats-streaming-concepts/ft/failover.md)
    - [Partitioning](../legacy/stan/nats-streaming-concepts/partitioning.md)
    - [Monitoring](../legacy/stan/nats-streaming-concepts/monitoring/README.md)
      - [Endpoints](../legacy/stan/nats-streaming-concepts/monitoring/endpoints.md)
  - [Developing With STAN](../legacy/stan/developing-with-nats-streaming/streaming.md)
    - [Connecting to NATS Streaming Server](../legacy/stan/developing-with-nats-streaming/connecting.md)
    - [Publishing to a Channel](../legacy/stan/developing-with-nats-streaming/publishing.md)
    - [Receiving Messages from a Channel](../legacy/stan/developing-with-nats-streaming/receiving.md)
    - [Durable Subscriptions](../legacy/stan/developing-with-nats-streaming/durables.md)
    - [Queue Subscriptions](../legacy/stan/developing-with-nats-streaming/queues.md)
    - [Acknowledgements](../legacy/stan/developing-with-nats-streaming/acks.md)
    - [The Streaming Protocol](../legacy/stan/developing-with-nats-streaming/protocol.md)
  - [STAN NATS Streaming Server](../legacy/stan/nats-streaming-server/changes.md)
    - [Installing](../legacy/stan/nats-streaming-server/install.md)
    - [Running](../legacy/stan/nats-streaming-server/run.md)
    - [Configuring](../legacy/stan/nats-streaming-server/configuring/README.md)
      - [Command Line Arguments](../legacy/stan/nats-streaming-server/configuring/cmdline.md)
      - [Configuration File](../legacy/stan/nats-streaming-server/configuring/cfgfile.md)
      - [Store Limits](../legacy/stan/nats-streaming-server/configuring/storelimits.md)
      - [Persistence](../legacy/stan/nats-streaming-server/configuring/persistence/README.md)
        - [File Store](../legacy/stan/nats-streaming-server/configuring/persistence/file_store.md)
        - [SQL Store](../legacy/stan/nats-streaming-server/configuring/persistence/sql_store.md)
      - [Securing](../legacy/stan/nats-streaming-server/configuring/tls.md)
    - [Process Signaling](../legacy/stan/nats-streaming-server/process-signaling.md)
    - [Windows Service](../legacy/stan/nats-streaming-server/windows-service.md)
    - [Embedding NATS Streaming Server](../legacy/stan/nats-streaming-server/embedding.md)
    - [Docker Swarm](../legacy/stan/nats-streaming-server/swarm.md)
    - [Kubernetes](../legacy/stan/nats-streaming-server/kubernetes/stan-kubernetes.md)
      - [NATS Streaming with Fault Tolerance.](../legacy/stan/nats-streaming-server/kubernetes/stan-ft-k8s-aws.md)
- [nats-account-server](../legacy/nas/README.md)
  - [Basics](../legacy/nas/nas_conf.md)
  - [Inspecting JWTs](../legacy/nas/inspecting_jwts.md)
  - [Directory Store](../legacy/nas/dir_store.md)
  - [Update Notifications](../legacy/nas/notifications.md)
