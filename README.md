# 2Captcha
2Captcha team solves your CAPTCHA with high accuracy

## How to install?

### Source
```
git clone https://github.com/cdn-db/captcha2upload.git
cd captcha2upload
python setup.py install
```

## How to start?
[Register Here](http://2captcha.com/?from=1083991)
And get the api key:
* Login in your account
* Go to "2Captcha API"
* Get "CAPTCHA Key"

# Example

## Solve Captcha
```
from captcha2upload import CaptchaUpload

captcha = CaptchaUpload(<YOURKEY>)
idCaptcha,captchaAnswer = captcha.solve(<PATHFILE>)
print idCaptcha
print captchaAnswer
```

## Report Bad Captcha Answer
```
from captcha2upload import CaptchaUpload

captcha = CaptchaUpload(<YOURKEY>)
print captcha.report(<IDCAPTCHA>)
```

## Get balance
```
from captcha2upload import CaptchaUpload

captcha = CaptchaUpload(<YOURKEY>)
print captcha.getbalance()
```

## Attach the logs
```
from captcha2upload import CaptchaUpload

captcha = CaptchaUpload(<YOURKEY>, log=<YOURLOGVAR>)
print captcha.getbalance()
```

## Change Wait Time
```
from captcha2upload import CaptchaUpload

captcha = CaptchaUpload(<YOURKEY>, waittime=<YOURLOGVAR>)
print captcha.solve(<PATHFILE>)
```

