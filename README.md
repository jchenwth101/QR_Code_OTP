Instructions for how to run the program:
-program was written in Python and can be run:

    -python OTP.py
    
    once running enter: --generate-qr and --get-otp
    scan the ironman_qrcode.jpg with google authenticator
    each 30 secs, the OTP should match the authenticator.

Implementation process:

I began by researching qr code generation and one-time password generation for Python Programming.
I found documentation on both and installed both libraries on pycharm: pip install qrcode 
and pip install pyotp.

From there, I was able to review documentation to identify how to encode the URI Google Authenticator expects
in the QR code as well as how to generate the QR code using the Python library. Much of the code
came from online sources.


Assumptions:
-User id for URI can be whatever the author chooses, in this case: ironman@avengers.com
-Secret key can be hard coded, I went with this randomly generated key: 5A4ZCQTANBGSY666
-Commands --generate-qr and --get-otp can be treated as input and entered after the program is running
-Testing using iOS Google Authenticator is sufficient as outlined in assignment: 

Future Considerations:
-Take validated user input for user id to make this more dynamic
-Generate a new, random secret key each time program is run
-Try different color combos for the QR code