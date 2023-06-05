import smtplib 

gmail_user ='darshanbambal813@gmail.com'
gmail_password ='****************'

sent_from = gmail_user
to = ['darshan812003@gmail.com']
subject = 'Testing of gmail sending by using python'
body = 'IT IS JUST FOR TESTING THE ONE OF THE APPLICATION OF PYTHON'

email_text = """\
From: %s
To: %s
Subject: %s

%s
""" % (sent_from, ", ".join(to), subject, body)


try:
    smtp_server = smtplib.SMTP_SSL('smtp.gmail.com', 587)
    smtp_server.ehlo()
    smtp_server.login(gmail_user, gmail_password)
    smtp_server.sendmail(sent_from, to, email_text)
    smtp_server.close()
    print ("Email sent successfully!")
except Exception as ex:
    print ("Something went wrong….",ex)
