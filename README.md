# HOW TO SETUP THIS EXAMPLE USING AUTH REQUEST

0. Create superuser: `python manage.py createsuperuser`
1. Migrate: `python manage.py migrate`
2. Start server: `python manage.py runserver <local-ip>:8000`
3. Change global.domain in lab/chart/values.yaml to `<local-ip>.nip.io`
4. Deploy lab: `helm install lab lab/chart`

Go to `http://<local-ip>.nip.io:8000` 
Login with the superuser created in step 0.

Go to `http://lab.<local-ip>.nip.io>`

Expected behaviour is that the auth subrequest from ingress controller should see that superuser is aleady loged in.
This is not the case for me.  
