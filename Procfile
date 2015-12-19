web: gunicorn -b 0.0.0.0:$PORT connect.wsgi
scheduler2: python manage.py celeryd -B -E --autoscale=1,7 --without-gossip --without-mingle
worker2: python manage.py celeryd -E --autoscale=1,7 --without-gossip --without-mingle
