#Federation API(server-server APIs)  文档翻译
####简介
1. matrix 服务器使用此APIs 在不同服务器中 发送信息，检索历史信息，查询彼此服务器上用户的状态和配置文件  
2. 这些api通过https请求实现。这些https请求使用TLS传输层的公钥和http层的认证头部的公钥进行身份认证
3. 服务器的交流有三种行为
   1. persisted Data Units(PDUs):信息从一个服务器广播给其他加入同一个聊天室的服务器。这些信息是持久存储的。记录了一个房间的历史消息和状态
   2. Ephemeral Data Units (EDUs):这些活动是在服务器之间进行的。它们不会一直存在，也不是房间历史的一部分，接收它们的服务器也不必回复它们。
   3. Queries: 用于查询一些信息。不会持续存在
4.edu和pdu进一步封装在一个称为Transaction的信封中，该信封使用HTTPS PUT请求从源服务器传输到目的地homeserver。
