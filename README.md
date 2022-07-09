# Mitre ATT&CK 구조

  
    1. ATT&CK Matrix
        – 공격 기술인 tactic, technique 개념과 관계를 시각화.
        – Tactic에는 다양한 technique가 포함.
        – 각 tactic는 공격 목표에 따라 다양함.  
  
    2. ATT&CK Tactics
        – 공격 목표에 따른 공격자의 행동을 나타냄.
        – 상황에 따른 각 technique에 대한 범주 역할.
        – 지속성, 정보탐색, 실행, 파일 추출 등 공격자의 목적에 따라 분류.
   
    3. ATT&CK Techniques
        – 공격자가 목표에 대한 tactic을 달성하기 위한 방법을 나타냄.
        – Technique을 사용함으로써 발생하는 결과(피해)를 명시.
        – Tactic에 따라 다양한 technique들이 존재할 수 있음.


# ATT&CK For Enterprise Matrix

    1. 구성 및 목적
        – 기업용 네트워크에 대한 14개의 tactic, 205개의 technique으로 카테고리별 목록화.
        – Cyber Kill Chain 모델의 단계 중 5단계(deliver, exploit, control, execute, maintain)에 해당.
        – 공격자의 TTP, 네트워크 공격 활동 특징 기반으로 작성.
        – Computer Network Defense (CND) 기술, 프로세스 및 정책을 종합적으로 평가.
 
    2. 활용
        – CND 개발 및 방어 우선순위 지정.- CND 간 기능 및 성능 분석.- CND 범위 설정.- 체계적 절차에 따른 intrusion에 대한 설명.- Mitigation과 연계, 취약점 분석.
 
    3. 지원 플랫폼
        – Windows, macOS, Linux
        – AWS, GCP, Azure, Azure AD, Office 365, SaaS       

# ATT&CK For Enterprise Tactics

    1. Tactics

        – TA0043 정찰 (Reconnaissance) 내부정찰단계로 다른시스템으로 이동하기 위해 탐구하는 단계
        – TA0042 자원 개발 (Resource Development) 다른시스템으로 이동하기 위한 정보로 계정 등을 확보하는 단계
        – TA0001 초기 접근 단계 (Initial Access) 네트워크 진입을 위해 사용자 환경에 대한 정보를 취득하는 것을 목적으로 함
        – TA0002 실행 (Execution) 공격자가 로컬 또는 원격 시스템을 통해 악성코드를 실행하기 위한 행동
        – TA0003 지속 (Persistence) 공격 기반을 유지하고 시스템에 지속적으로 접근하기 위한 행동
        – TA0004 권한 상승 (Privilege Escalation) 공격자가 시스템이나 네트워크에서 높은 권한을 얻기 위한 행동
        – TA0005 방어 회피 (Defense Evasion) 공격자가 침입한 시간 동안 탐지 당하는 것을 피하기 위한 행동
        – TA0006 접속 자격 증명 (Credential Access) 시스템, 도메인 서비스, 자격증명 등을 접근하거나 제어하기 위한 행동
        – TA0007 탐색 (Discovery) 시스템 및 내부 네트워크의 정보를 얻기 위한 행동
        – TA0008 내부 확산 (Lateral Movement) 네트워크 상의 원격 시스템에 접근한 후 이를 제어하기 위한 행동
        – TA0009 수집 (Collection) 공격 목적이나 관련 정보가 포함된 데이터를 수집하기 위한 행동
        – TA0011 명령 및 제어(Command And Control) 공격자가 침입한 대상 네트워크 내부 시스템과 통신하며 제어하기 위한 행동
        – TA0010 유출 (Exfiltration) 공격자가 네트워크에서 데이터를 훔치기 위한 행동
        – TA0040 임팩트 (Impact) 공격 목표의 가용성과 무결성을 손상시키기 위한 행동

    2. Techniques

        – 초기 접근 단계 (Initial Access) Valid Account, Exploit Public-Facing Application, Supply Chain Compromise, Drive-By Compromise, SpearPhishing Link / Attachment
        
        – 실행 (Execution) Command-Line Interface, PowerShell Scripting, WMI, Graphical User Interface, Rundll32, Scheduled Task, Service Execution
        
        – 지속 (Persistence) Valid Accounts, Web Shell, Registry Run Key / Startup Folder, Scheduled Task, New Service, Create Account, Account Manipulation
        
        – 방어 회피 (Defense Evasion) Valid Accounts, Scripting, Masquerading, Disabling Security Tools, File Deletion, Obfuscated Files or Information, Process Injection, Rundll32
        
        – 내부 확산 (Lateral Movement) Windows Admin Shares, Remote File Copy, Remote Desktop Protocol, Remote Service, WMI
