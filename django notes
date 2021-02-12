*This file is for help in django*

# Model

@import:
from django.db import models

EX:

class Snippet(models.Model):

	created = models.DateTimeField(auto_now_add= True)
	title = models.CharField(max_length=100, blank=True, default= '')
	code = models.TextField()
	linenos = models.BooleanField(default=False)

	class Meta:
		ordering = ['created']
