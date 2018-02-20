Credits to [ckelly](https://github.com/ckelly) on this repository: [django-resume](https://github.com/ckelly/django-resume) . 
The project was not working on python 3 and Django 2.0.2.


Fire up a shell and create your resume with commands similar to the following ones: 
```
from resume.models import Overview
over=Overview.objects.create(text='This is a test overview for this CV')
from resume.models import 

from resume.models import PersonalInfo
pi=PersonalInfo.objects.create('email': 'AlessandroMarin80@gmail.com', 'region': 'Massachusetts', 'region_shorthand': 'MA', 'first_name': 'Alessandro', 'locality': 'Boston', 'last_name': 'Marin')
pi.linkedin='https://www.linkedin.com/in/alessandromarin80/'
pi.save()

from resume.models import Education
sks=Skillset.objects.create(name='Programming Languages')
sks.save()
s1=Skill.objects.create(name='Python',skillset=sks)
s2=Skill.objects.create(name='Django',skillset=sks)


date=datetime.date(year=2018,month=2,day=19)
date2=datetime.date(year=2018,month=2,day=20)
j=Job.objects.create(company='MyCompany',start_date=date,completion_date=date2)
j.company='my company'
j.company_url='www.google.com'
j.__dict__

from resume.models import Education
Education.objects.create(name='University Somewhere',start_date=date,completion_date=date2)

```