web: gunicorn -b 0.0.0.0:$PORT connect.wsgi
# scheduler: NEW_RELIC_CONFIG_FILE=/app/newrelic-celery.ini bin/start-pgbouncer-stunnel newrelic-admin run-program python manage.py celeryd -B -E --autoscale=1,7 --without-gossip --without-mingle
# worker: NEW_RELIC_CONFIG_FILE=/app/newrelic-celery.ini bin/start-pgbouncer-stunnel newrelic-admin run-program python manage.py celeryd -E --autoscale=1,7 --without-gossip --without-mingle

scheduler2: python manage.py celeryd -B -E --autoscale=1,7 --without-gossip --without-mingle
worker2: python manage.py celeryd -E --autoscale=1,7 --without-gossip --without-mingle
