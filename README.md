# AdhiraCOA
# Import the following modules
from captcha.audio import AudioCaptcha

# Create an audio instance
audio = AudioCaptcha()
# captcha = AudioCaptcha(voicedir='/path/to/voices')

# Audio captcha text
captcha_text = '5454'

# Generate the audio of the given text
audio_data = audio.generate(captcha_text)

# Give the name of the audio file
audio_file = 'audio_' + captcha_text + '.wav'

# Finally write the audio file and save it
audio.write(captcha_text, audio_file)
