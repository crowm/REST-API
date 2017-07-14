# REST-API

Get Employee list using REST API

=========================
API:
=========================


URL    : <SERVER_URL>/get/api/1.0/get/list/employees
Header : {"Authorization", "OAuth <AUTHENTICATION_TOKEN>"}


=========================
REQUEST:
=========================

import urllib2

request = urllib2.Request('http://192.168.0.123:8989/get/api/1.0/get/list/employees')
request.add_header("Authorization", "OAuth Rhvs7vGZK59ggnYt6nJN2xNZLYcSL8dItvcmAYzgcmkGtzHI195UwahJlm-v5djPY37iZkfl8IL")
request = urllib2.urlopen(request)
result = request.read()


=========================
RESPONSE:
=========================

{u'employees': [{u'active': True,
                 u'city': False,
                 u'coach_id': False,
                 u'company_id': 1,
                 u'country_id': False,
                 u'department_id': 4,
                 u'gender': u'male',
                 u'id': 2,
                 u'job_id': 2,
                 u'marital': u'single',
                 u'name': u'Antoine Langlais',
                 u'user_id': False,
                 u'work_phone': u'+3281813700'},
                {u'active': True,
                 u'city': False,
                 u'coach_id': False,
                 u'company_id': 1,
                 u'country_id': False,
                 u'department_id': 1,
                 u'gender': False,
                 u'id': 12,
                 u'job_id': 5,
                 u'marital': False,
                 u'name': u'Ashley Presley',
                 u'user_id': False,
                 u'work_phone': u'+3281813700'}]}
