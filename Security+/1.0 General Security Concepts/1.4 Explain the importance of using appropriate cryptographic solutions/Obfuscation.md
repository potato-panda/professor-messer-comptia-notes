### The process of making something unclear
- it's now much more difficult to understand
### But it's not impossible to understand
- if you know how to read it
### Hide information in plain sight
- store payment info without storing a credit card number
### Hide information inside of an image
- steganography
# Steganography
### Greek for "concealed writing"
- security through obscurity
### Message is invisible
- but it's really there
### The covertest
- the container document or file
# Common steganography techniques
### Network based
- embed messages in TCP packets
### Use an image
- embed message in image
### Invisible watermarks
- yellow dots on printers
# Other steganography types
### Audio
- modify the digital audio file
- interlace a secret message within the audio
- similar technique to image steganography
### Video
- a sequence of image
- use image steganography on a larger scale
- manage the signal to noise ratio
- potentially transfer much more info
# Tokenization
### Replace sensitive data with a non-sensitive placeholder
- SSN 266-12-1112 is now 691-61-8539
### Common with credit card processing
- use a temp token during payment
- an attacker capturing the card numbers can't use them later
### This isn't encryption or hashing
- the original data and token aren't mathematically related
![[Pasted image 20240605144257.png]]
# Data masking
### Data obfuscation
- hide some of the original data
### Protects PII
- and other sensitive data
### May only be hidden from view
- the data may still be intact in storage
- control the view based on permissions
![[Pasted image 20240605144356.png]]
### Many different techniques
- substituting, shuffling, encrypting, masking out, etc