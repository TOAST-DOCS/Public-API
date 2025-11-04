# Public API 개요

**Public API > Public API 개요**

NHN Cloud의 Public API는 NHN Cloud에서 제공하는 서비스와 리소스를 외부 시스템 또는 사용자 애플리케이션에서 제어하거나 연동할 수 있도록 지원하는 HTTP 기반 인터페이스입니다.

[개요 이미지 추가: NHN Cloud_Guide overview_PublicAPI_v2_ko]

이 문서는 Public API 호출 시 필요한 인증 방법과 서비스별 인증 방식 지원 현황, 프레임워크 API 등 Public API를 사용하기 위한 전반에 대해 설명합니다. NHN Cloud의 Public API를 연동하고자 하는 개발자, API 인증 방식의 종류와 사용 방식을 이해하고자 하는 서비스 기획자, API를 통해 NHN Cloud 리소스를 자동화하고자 하는 시스템 운영자가 이 문서를 활용할 수 있습니다.

!!! tip "알아두기"
    * 서비스별 API 세부 동작과 응답 형식은 해당 서비스의 API 가이드를 참고하세요.
    * 서비스마다 지원하는 API 인증 방식이 다르며, 일부 인증 방식은 특정 서비스에서만 지원합니다. 서비스별 지원되는 인증 방식은 [서비스별 인증 방식](link 입력)에서 확인할 수 있습니다.

## Public API 시작하기
* [인증 방식](link 입력)
* [서비스별 인증 방식](link 입력)
* [프레임워크 API](https://docs.nhncloud.com/ko/nhncloud/ko/public-api/framework-api/)
* [파트너 관리 API](https://docs.nhncloud.com/ko/nhncloud/ko/public-api/partner-api/)
* [릴리스 노트](https://docs.nhncloud.com/ko/nhncloud/ko/public-api/release-notes/)

## 용어 정리

| 용어 | 설명 |
| --- | --- |
| Public API | NHN Cloud에서 제공하는 REST API로, NHN Cloud 서비스와 리소스를 외부 시스템 또는 사용자 애플리케이션에서 제어하거나 연동할 수 있도록 지원 |
| 프레임워크 API | 클라우드의 조직과 프로젝트를 관리하는 API |
| 파트너 관리 API | NHN Cloud 파트너 또는 파트너에게 권한을 부여 받은 사용자가 파트너 클라우드의 조직과 프로젝트, 빌링 등을 관리하고 상품 미터링을 조회할 수 있는 API |
| 인증(Authentication) | 어떤 주체의 신원을 확인하고 증명함 |
| 인가(Authorization) | 인증을 통해 신원이 확인된 주체에게 특정 리소스나 기능에 접근하거나 동작을 수행할 권한이 있는지 확인하고 허용하는 과정 |
| Bearer 토큰 | 토큰을 소유한 사용자에게 접근 권한을 부여하는 보안 토큰의 유형 | 
| Keystone | OpenStack의 인증 및 권한 부여 작업을 담당하는 서비스. 사용자와 서비스의 신원을 확인하고 적절한 권한을 부여하여 리소스에 대한 안전한 접근을 보장함 |



