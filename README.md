# HOW TO SETIP THIS EXAMPLE USING AUTH REQUEST

1. Start server: python manage.py runserver <local-ip>:8000
2. Change global.domain in lab/chart/values.yaml to <local-ip>.nip.io
3. Deploy lab: helm install lab lab/chart 
