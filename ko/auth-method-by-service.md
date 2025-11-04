# 서비스별 인증 방식

**Public API > 서비스별 인증 방식**

NHN Cloud의 Public API는 인증을 위해 User Access Key 토큰, IaaS 토큰, User Access Key, Appkey, 프로젝트 통합 Appkey를 지원합니다.
서비스마다 지원하는 API 인증 방식이 다르며, 일부 인증 방식은 특정 서비스에서만 지원합니다.

## 서비스별 인증 방식 확인하기
사용할 서비스에서 지원하는 API 인증 방식을 확인하세요.


| Category                | Service                      | Appkey | 프로젝트 통합 Appkey | User Access Key | User Access Key 토큰 | IaaS 토큰 |
| ----------------------- | ---------------------------- | ------ | -------------------- | --------------- | --------------------- | ---------- |
| **Compute**             | Instance                     |        |                      |                 |                       | O          |
|                         | GPU Instance                 |        |                      |                 |                       |            |
|                         | Instance Template            |        |                      |                 |                       |            |
|                         | Image                        |        |                      |                 |                       | O          |
|                         | Image Builder                |        |                      |                 |                       |            |
|                         | Auto Scale                   |        |                      |                 |                       |            |
|                         | Virtual Desktop              |        |                      |                 |                       |            |
|                         | Cloud Functions              |        |                      |                 |                       |            |
| **Container**           | NHN Kubernetes Service (NKS) |        |                      |                 |                       | O          |
|                         | NHN Container Registry (NCR) | ~~O~~  |                      | O               |                       |            |
|                         | NHN Container Service (NCS)  |        |                      |                 | O                     |            |
| **Network**             | VPC                          |        |                      |                 |                       | O          |
|                         | Network Interface            |        |                      |                 |                       |            |
|                         | Flow Log                     |        |                      |                 |                       | O          |
|                         | Floating IP                  |        |                      |                 |                       | O          |
|                         | Network ACL                  |        |                      |                 |                       | O          |
|                         | Security Groups              |        |                      |                 |                       | O          |
|                         | Load Balancer                |        |                      |                 |                       | O          |
|                         | NAT Instance                 |        |                      |                 |                       |            |
|                         | Transit Hub                  |        |                      |                 |                       | O          |
|                         | Internet Gateway             |        |                      |                 |                       |            |
|                         | Peering Gateway              |        |                      |                 |                       |            |
|                         | Colocation Gateway           |        |                      |                 |                       |            |
|                         | NAT Gateway                  |        |                      |                 |                       |            |
|                         | VPN Gateway(Site-to-Site VPN)|        |                      |                 |                       |            |
|                         | Service Gateway              |        |                      |                 |                       | O          |
|                         | Traffic Mirroring            |        |                      |                 |                       |            |
|                         | Private DNS                  |        |                      |                 |                       |            |
|                         | DNS Plus                     | O      | O                    |                 |                       |            |
|                         | Direct Connect               |        |                      |                 |                       |            |
| **Storage**             | Block Storage                |        |                      |                 |                       | O          |
|                         | NAS                          |        |                      |                 |                       |            |
|                         | NAS offline                  |        |                      |                 |                       |            |
|                         | NAS for AI                   |        |                      |                 |                       |            |
|                         | Object Storage<span style="color:red">*</span> |        |                      |                 |                       | O          |
|                         | Backup                       |        |                      |                 |                       |            |
|                         | Storage Gateway              |        |                      |                 |                       |            |
|                         | Data Transporter             |        |                      |                 |                       |            |
| **Database**            | RDS for MySQL                | O      | O                    | O               |                       |            |
|                         | RDS for MariaDB              | O      | O                    | O               |                       |            |
|                         | RDS for MS-SQL               |        |                      |                 |                       |            |
|                         | RDS for PostgreSQL           |        |                      |                 | O                     |            |
|                         | EasyCache                    |        |                      |                 |                       |            |
| **Monitoring**          | Service Monitoring           | O      |                      |                 |                       |            |
|                         | Cloud Monitoring             |        |                      |                 |                       |            |
| **Game**                | Gamebase                     | O      |                      |                 |                       |            |
|                         | GameAnvil                    |        |                      |                 |                       |            |
|                         | GameStarter                  |        |                      |                 |                       |            |
|                         | Leaderboard                  | O      |                      |                 |                       |            |
|                         | Launching                    | O      |                      |                 |                       |            |
| **Security**            | NHN AppGuard                 | O      |                      | O               |                       |            |
|                         | Server Security Check        | O      |                      |                 |                       |            |
|                         | Webshell Threat Detector     | O      |                      |                 |                       |            |
|                         | Security Monitoring          | O      |                      |                 |                       |            |
|                         | WEB Firewall                 |        |                      |                 |                       |            |
|                         | Vaccine                      |        |                      |                 |                       |            |
|                         | Security Compliance          | O      |                      |                 |                       |            |
|                         | Security Advisor             | O      |                      |                 |                       |            |
|                         | Network Firewall             |        |                      |                 |                       |            |
|                         | NHN Bastion                  | O      |                      |                 |                       |            |
|                         | Secure Key Manager           | O      | O                    | O               |                       |            |
|                         | Cloud Access                 |        |                      |                 |                       |            |
| **Content Delivery**    | CDN                          | O      | O                    |                 |                       |            |
|                         | Image Manager                | O      | O                    |                 |                       |            |
| **Notification**        | Push                         | O      |                      |                 |                       |            |
|                         | SMS                          | O      |                      |                 |                       |            |
|                         | RCS Bizmessage               | O      |                      |                 |                       |            |
|                         | Email                        | O      |                      |                 |                       |            |
|                         | KakaoTalk Bizmessage         | O      |                      |                 |                       |            |
|                         | Notification Hub             |        |                      |                 | O                     |            |
| **AI Service**          | Face Recognition             | O      |                      |                 |                       |            |
|                         | AI Fashion                   | O      |                      |                 |                       |            |
|                         | OCR                          | O      |                      |                 |                       |            |
|                         | Text to Speech               | O      |                      |                 |                       |            |
|                         | Speech to Text               | O      |                      |                 |                       |            |
| **Machine Learning**    | AI EasyMaker                 | O      | O                    |                 |                       |            |
| **Application Service** | ROLE                         | O      | O                    |                 |                       |            |
|                         | API Gateway                  | O      | O                    |                 |                       |            |
|                         | RTCS                         | O      |                      |                 |                       |            |
|                         | ShortURL                     | O      |                      |                 |                       |            |
|                         | File-Crafter                 | O      |                      |                 |                       |            |
|                         | Cloud Scheduler              |        |                      |                 |                       |            |
| **Mobile Service**      | IAP                          | O      |                      |                 |                       |            |
| **Search**              | Cloud Search                 | O      |                      |                 |                       |            |
|                         | Autocomplete                 | O      |                      |                 |                       |            |
|                         | Corporation Search           | O      |                      |                 |                       |            |
| **Data & Analytics**    | Log & Crash Search           | O      |                      |                 |                       |            |
|                         | DataFlow                     |        |                      |                 |                       |            |
|                         | DataQuery                    |        |                      |                 |                       |            |
| **Dev Tools**           | Pipeline                     |        |                      | O               |                       |            |
|                         | Deploy                       | O      |                      | O               |                       |            |
| **Management**          | Managed                      |        |                      |                 |                       |            |
|                         | Certificate Manager          | O      |                      | O               |                       |            |
| **Contact Center**      | Contiple                     | O      |                      |                 |                       |            |
|                         | Mobile Contact               |        |                      |                 |                       |            |
| **Governance & Audit**  | CloudTrail                   | O      |                      | O               |                       |            |
|                         | Resource Watcher             | O      |                      | O               |                       |            |


!!! tip "알아두기"
    <span style="color:red">*</span> Object Storage 서비스는 AWS의 Amazon S3 API와 호환되는 API를 제공합니다. Amazon S3 호환 API를 사용하려면 AWS EC2 형태의 S3 API 자격 증명을 발급해야 합니다. S3 API 자격 증명에 대한 자세한 설명은 [S3 API 자격 증명(S3 API Credential)](https://docs.nhncloud.com/ko/Storage/Object%20Storage/ko/s3-api-guide/#s3-api-s3-api-credential)에서 확인할 수 있습니다.



