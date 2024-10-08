*This file is for help in DRF*

# Serializers

@import:
from rest_framework import serializers


EX:

class FirstSnippetSerializer(serializers. Serializer):

	id 		= serializers.IntegerField(read_only = True)
	title		= serializers.CharField(required=False, allow_blank = True, max_length = 100)
	code		= serializers.CharField(style={'base_template': 'textarea.html'})
	linenos 	= serializers.BooleanField(required=False)
	language 	= serializers.ChoiceField(choices = LANGUAGE_CHOICES, default = 'python')
	style 		= serializers.ChoiceField(choices = STYLE_CHOICES, default = 'friendly')

	def create(self, validated_data):
		return Snippet.objects.create(**validated_data)

	def update(self, instance, validated_data):
		instance.title 		= validated_data.get('title', instance.title)
		instance.code 		= validated_data.get('code', instance.code)
		instance.linenons 	= validated_data.get('linenons', instance.linenons)
		instance.language 	= validated_data.get('language', instance.language)
		instance.style 		= validated_data.get('style', instance.style)
		instance.save()
		return isinstance;

EX:

class SnippetSerializer(serializers.ModelSerializer):

	class Meta:
		model 	= Snippet
		fields 	= ['title', 'code', 'language','style']


