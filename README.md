# system_collctor

## 모니터링 시스템 상태 점검 시스템

1. monitor.py
   ㄴ 윈도우 작업스케줄러에서 1분마다 실행
   ㄴ 시스템 DOWN(3분) / 재일림(30분) / 복구 알림 1회 진행
   ㄴ 알림 폭주 방지를 위해 gabia db의 tb_system_collector_alert_state 테이블 사용
   ㄴ 알럿 리스트 조회의 경우 gabia db의 tb_system_collector_heartbeat 테이블 사용
