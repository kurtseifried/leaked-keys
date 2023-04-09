export API_KEY="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"

OpenAI: sub 1 minute response time:

Original Message
Message ID	<31165340.20230409030545.64322b8902eaf0.25359411@mail6.wdc04.mandrillapp.com>
Created at:	Sat, Apr 8, 2023 at 9:05 PM (Delivered after 0 seconds)
From:	OpenAI <noreply@tm.openai.com>
To:	kurt@seifried.org
Subject:	OpenAI API - API Key Disabled
SPF:	PASS with IP 205.201.139.6 Learn more
DKIM:	'PASS' with domain tm.openai.com Learn more
DMARC:	'PASS' Learn more


Download Original	Copy to clipboard	
Delivered-To: kurt@seifried.org
Received: by 2002:a05:6504:598:b0:225:7bff:541c with SMTP id i24csp1126282lto;
        Sat, 8 Apr 2023 20:05:45 -0700 (PDT)
X-Google-Smtp-Source: AKy350Y5se1gu7biKEBSsm20XKgSdJfYOrgR62e/fHPXD+TSyD4odrYDiHdpUejqTRTh2sbber7Q
X-Received: by 2002:a0d:e447:0:b0:545:f5e2:254b with SMTP id n68-20020a0de447000000b00545f5e2254bmr5087848ywe.14.1681009545350;
        Sat, 08 Apr 2023 20:05:45 -0700 (PDT)
ARC-Seal: i=1; a=rsa-sha256; t=1681009545; cv=none;
        d=google.com; s=arc-20160816;
        b=L0yPRFA7keBDCSQsYnqnMuIImJTkGcMucv8UZwHJXnEz26QIUUUuYI7fOMbdBT2ehY
         QR42W+NXiu4DSdOmb52GX60KpZUTCYpax0thXDj/YUzaU9WPOiWlOokRTkPEsIFXe0S8
         0cEYk8NQY9V0TaeSk/yMEyFU5GmihIHi5cl3SlZStufAf8o9ubSWdFxzxKSTs2ygkr8l
         EGHxmYV9sYXzKXHNzVIT7sQzzPLvo/bgbIu80u4v323wrv6ZRknwxa0iHHE5DpF23iBq
         5guC7RtgrxvxmAdGvrsy/WjsHusbZlm19P0LRN+tUzl96whDyhfMQ1fJWYgFYxCpOtxt
         j/+g==
ARC-Message-Signature: i=1; a=rsa-sha256; c=relaxed/relaxed; d=google.com; s=arc-20160816;
        h=mime-version:date:message-id:feedback-id:to:reply-to:subject:from
         :dkim-signature:dkim-signature;
        bh=QhkeRYxlOhEw0Di2zWOiq/3WqmAAgg6vf+hcbmMi7G4=;
        b=x1F/1X/5cbXiPYLFkrjCkh1deIvy/0zqvpSoP/lCaOI9KbzYY4zIj3zFTlcDBpi41g
         7EDNaLyzN+BAJkGPJvuR9pVUpDKofEfKx9nw31QyBbRsKHh88pAP23pA4Z+O240TScnK
         1/UHxFt7UXWpnVXlSeszwPXlG5RM1g61hTmL3mElAwtoRtJ2w534ssnwAjeeanQr4VS+
         WFpCXqaAcfsVx4SHm0hYbJ7w7Z5vrxF9Yr5XWXr9Nvf9L/HlfT5L5ArbxjT1rDxEAws1
         CCSQocC+3W9YHbGkAGmAe9ybNoiczpCmgJZviq7datrAxF6mvoR4pmb3Xww5quwH3SHM
         lIWg==
ARC-Authentication-Results: i=1; mx.google.com;
       dkim=pass header.i=@tm.openai.com header.s=mandrill header.b=kiOS5SDb;
       dkim=pass header.i=@mandrillapp.com header.s=mandrill header.b=qRuDknxQ;
       spf=pass (google.com: domain of bounce-md_31165340.64322b88.v1-ce7e5305332549f7afe94f815a970eb5@mandrillapp.com designates 205.201.139.6 as permitted sender) smtp.mailfrom=bounce-md_31165340.64322b88.v1-ce7e5305332549f7afe94f815a970eb5@mandrillapp.com;
       dmarc=pass (p=REJECT sp=REJECT dis=NONE) header.from=openai.com
Return-Path: <bounce-md_31165340.64322b88.v1-ce7e5305332549f7afe94f815a970eb5@mandrillapp.com>
Received: from mail6.wdc04.mandrillapp.com (mail6.wdc04.mandrillapp.com. [205.201.139.6])
        by mx.google.com with ESMTPS id g186-20020a816bc3000000b0052eb827d057si6967098ywc.12.2023.04.08.20.05.45
        for <kurt@seifried.org>
        (version=TLS1_3 cipher=TLS_AES_256_GCM_SHA384 bits=256/256);
        Sat, 08 Apr 2023 20:05:45 -0700 (PDT)
Received-SPF: pass (google.com: domain of bounce-md_31165340.64322b88.v1-ce7e5305332549f7afe94f815a970eb5@mandrillapp.com designates 205.201.139.6 as permitted sender) client-ip=205.201.139.6;
Authentication-Results: mx.google.com;
       dkim=pass header.i=@tm.openai.com header.s=mandrill header.b=kiOS5SDb;
       dkim=pass header.i=@mandrillapp.com header.s=mandrill header.b=qRuDknxQ;
       spf=pass (google.com: domain of bounce-md_31165340.64322b88.v1-ce7e5305332549f7afe94f815a970eb5@mandrillapp.com designates 205.201.139.6 as permitted sender) smtp.mailfrom=bounce-md_31165340.64322b88.v1-ce7e5305332549f7afe94f815a970eb5@mandrillapp.com;
       dmarc=pass (p=REJECT sp=REJECT dis=NONE) header.from=openai.com
DKIM-Signature: v=1; a=rsa-sha256; c=relaxed/relaxed; d=tm.openai.com; s=mandrill; t=1681009545; x=1681067145; i=noreply@tm.openai.com; bh=QhkeRYxlOhEw0Di2zWOiq/3WqmAAgg6vf+hcbmMi7G4=; h=From:Subject:Reply-To:To:Feedback-ID:Message-Id:Date:MIME-Version:
	 Content-Type:CC:Date:Subject:From; b=kiOS5SDbsKbrRb4C5Ms39UfsDbTLcaRBm2KIIuxjXOJMGgo0PGKMtz5/+vscFSogf
	 INKucYjaZvVXHRytMY+fDMSYf8FNKy0GsfxiV+hzikTK3GUQDTHMkdpPq6RW87FCkK
	 f3NffXuFkBTmfykGBQVA0XmizaMk67H6uZTKWUI8=
Received: from pmta16.mandrill.prod.suw01.rsglab.com (localhost [127.0.0.1]) by mail6.wdc04.mandrillapp.com (Mailchimp) with ESMTP id 4PvH6d0T48z2K2SF6 for <kurt@seifried.org>; Sun,
  9 Apr 2023 03:05:45 +0000 (GMT)
DKIM-Signature: v=1; a=rsa-sha256; c=relaxed/relaxed; d=mandrillapp.com;
  i=@mandrillapp.com; q=dns/txt; s=mandrill; t=1681009545; h=From :
  Subject : Reply-To : To : Message-Id : Date : MIME-Version :
  Content-Type : From : Subject : Date : X-Mandrill-User :
  List-Unsubscribe; bh=QhkeRYxlOhEw0Di2zWOiq/3WqmAAgg6vf+hcbmMi7G4=;
  b=qRuDknxQ7o57j+wYtJcasD97tFWCnaZvgSPeDXWG74Q/dk3Shv6BzFue7Z/fFL+7VA7JI9 0kh8TxGSqnn/uvFgRwA1360A7pcl9CP++q0r+Va6XjtA3jrueVCGZPosV+XRGBWciakKjj+c YVuzSY+fGREiMWu0ibHhcNe6sBBUs=
From: OpenAI <noreply@tm.openai.com>
Subject: OpenAI API - API Key Disabled
Received: from [40.84.182.40] by mandrillapp.com id ce7e5305332549f7afe94f815a970eb5; Sun, 09 Apr 2023 03:05:44 +0000
Reply-To: support@openai.com
To: kurt@seifried.org
X-Native-Encoded: 0
X-Report-Abuse: Please forward a copy of this message, including all headers, to abuse@mandrill.com
X-Report-Abuse: You can also report abuse here: http://mandrillapp.com/contact/abuse?id=31165340.ce7e5305332549f7afe94f815a970eb5
X-Mandrill-User: md_31165340
Feedback-ID: 31165340:31165340.20230409:md
Message-Id: <31165340.20230409030545.64322b8902eaf0.25359411@mail6.wdc04.mandrillapp.com>
Date: Sun, 09 Apr 2023 03:05:45 +0000
MIME-Version: 1.0
Content-Type: multipart/alternative; boundary="_av-J7ojrq0M1BH4skdrgwiemw"

--_av-J7ojrq0M1BH4skdrgwiemw
Content-Type: text/plain; charset=utf-8
Content-Transfer-Encoding: 7bit

     OpenAI API - API Key Disabled      Your OpenAI API key has been
disabled 
                       Hi there, 

  Your OpenAI API key was determined to have been leaked, which has
triggered a key disable and this friendly notification email. 

  This may be because you committed your API key to an online service such
as GitHub, or your key may have been compromised in another way. 

  Don't worry, you still have API access! Head over to the API Keys
<https://platform.openai.com/account/api-keys> page to create a new API
key. 

  If your API key was stored in any locations - for instance, in code you
are running - it will need to be updated before you can run this code
again. 

  Finally, we ask that you please review our best practices for API key
safety
<https://help.openai.com/en/articles/5112595-best-practices-for-api-key-safety>.


  Best,
 The OpenAI team 

               If you have any questions please contact us through our help
center <https://help.openai.com/en/>
--_av-J7ojrq0M1BH4skdrgwiemw
Content-Type: text/html; charset=utf-8
Content-Transfer-Encoding: 7bit

<!DOCTYPE html>
<html>
<head>
  
  <meta charset="utf-8">
  <meta http-equiv="x-ua-compatible" content="ie=edge">
  <title>OpenAI API - API Key Disabled</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style type="text/css">
  /**
   * Google webfonts. Recommended to include the .woff version for cross-client compatibility.
   */
  @media screen {
    @font-face {
      font-family: Colfax;
      src: url(https://openai-public.s3-us-west-2.amazonaws.com/beta/fonts/ColfaxAIRegular.woff2);
      font-weight: normal;
    }

    @font-face {
      font-family: Colfax;
      src: url(https://openai-public.s3-us-west-2.amazonaws.com/beta/fonts/ColfaxAIMedium.woff2);
      font-weight: bold;
    }
  }

  /**
   * Avoid browser level font resizing.
   * 1. Windows Mobile
   * 2. iOS / OSX
   */
  body,
  table,
  td,
  a {
    -ms-text-size-adjust: 100%; /* 1 */
    -webkit-text-size-adjust: 100%; /* 2 */
    font-family: Colfax, Helvetica, Arial, sans-serif;
  }

  /**
   * Remove extra space added to tables and cells in Outlook.
   */
  table,
  td {
    mso-table-rspace: 0pt;
    mso-table-lspace: 0pt;
  }

  /**
   * Better fluid images in Internet Explorer.
   */
  img {
    -ms-interpolation-mode: bicubic;
  }

  /**
   * Remove blue links for iOS devices.
   */
  a[x-apple-data-detectors] {
    font-family: inherit !important;
    font-size: inherit !important;
    font-weight: inherit !important;
    line-height: inherit !important;
    color: inherit !important;
    text-decoration: none !important;
  }

  /**
   * Fix centering issues in Android 4.4.
   */
  div[style*="margin: 16px 0;"] {
    margin: 0 !important;
  }

  body {
    width: 100% !important;
    height: 100% !important;
    padding: 0 !important;
    margin: 0 !important;
  }

  /**
   * Collapse table borders to avoid space between cells.
   */
  table {
    border-collapse: collapse !important;
  }

  a {
    color: #10A37F;
  }

  img {
    height: auto;
    line-height: 100%;
    text-decoration: none;
    border: 0;
    outline: none;
  }

  h1 {
      font-size: 26px;
      line-height: 1.4;
      font-weight: 700;
      margin: 0;
  }
  h2 {
      font-size: 24px;
      line-height: 1.4;
      font-weight: 700;
      margin: 0;
  }
  p {
      margin: 0;
  }
  p + p {
      margin-top: 16px;
  }
  </style>

  
</head>
<body style="background-color:#ffffff;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;width:100% ;height:100% ;padding:0 ;margin:0 ;">

  <div class="preheader" style="display: none; max-width: 0; max-height: 0; overflow: hidden; font-size: 1px; line-height: 1px; color: #fff; opacity: 0;">
      Your OpenAI API key has been disabled
  </div>

  <!-- start body -->
  <table border="0" cellpadding="0" cellspacing="0" width="100%" style="-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;border-collapse:collapse ;">
    <!-- start body block -->
    <tr>
      <td align="center" style="-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;">
        <!--[if (gte mso 9)|(IE)]>
        <table align="center" border="0" cellpadding="0" cellspacing="0" width="600">
        <tr>
        <td align="center" valign="top" width="600">
        <![endif]-->
        <table border="0" cellpadding="0" cellspacing="0" width="100%" style="width:560px;background-color:#fff;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;border-collapse:collapse ;">
            <!-- header image -->
            <tr>
                <td valign="top" style="padding:27px 20px 24px 15px;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;">
                    <table align="left" width="100%" border="0" cellpadding="0" cellspacing="0" style="min-width:100%;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;border-collapse:collapse ;">
                        <tbody><tr>
                            <td valign="top" style="padding-top:0;padding-bottom:0;text-align:left;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;">
                                <img align="left" alt="" src="https://cdn.openai.com/API/logo-assets/openai-logo-email-header-1.png" width="560" height="168" style="width:140px;max-width:100%;padding-bottom:0;display:inline !important;vertical-align:bottom;-ms-interpolation-mode:bicubic;height:auto;line-height:100%;text-decoration:none;border:0;outline:none;">
                            </td>
                        </tr>
                        </tbody></table>
                </td>
            </tr>

          
<tr>
  <td align="left" bgcolor="#ffffff" style="padding:16px 24px;font-size:16px;line-height:24px;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;">
    <p style="margin:0;">
      Hi there,
    </p>
    <p style="margin:0;margin-top:16px;">
      Your OpenAI API key was determined to have been leaked, which has triggered a key disable and this friendly notification email.
    </p>
    <p style="margin:0;margin-top:16px;">
      This may be because you committed your API key to an online service such as GitHub, or your key may have been compromised in another way.
    </p>
    <p style="margin:0;margin-top:16px;">
      Don't worry, you still have API access! Head over to the <a href="https://mandrillapp.com/track/click/31165340/platform.openai.com?p=eyJzIjoiVU9rbnNSRDBHWEo4cDh0OHNHakVKMGxDZnpnIiwidiI6MSwicCI6IntcInVcIjozMTE2NTM0MCxcInZcIjoxLFwidXJsXCI6XCJodHRwczpcXFwvXFxcL3BsYXRmb3JtLm9wZW5haS5jb21cXFwvYWNjb3VudFxcXC9hcGkta2V5c1wiLFwiaWRcIjpcImNlN2U1MzA1MzMyNTQ5ZjdhZmU5NGY4MTVhOTcwZWI1XCIsXCJ1cmxfaWRzXCI6W1wiZGRlMTIyMmY1ZjBmNGVlOWEwNGY2NzdkZDQ2N2ZjN2MyNTllN2U4MFwiXX0ifQ" target="_blank" style="-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;color:#10A37F;">API Keys</a> page to create a new API key.
    </p>
    <p style="margin:0;margin-top:16px;">
      If your API key was stored in any locations - for instance, in code you are running - it will need to be updated before you can run this code again.
    </p>
    <p style="margin:0;margin-top:16px;">
      Finally, we ask that you please review our <a href="https://mandrillapp.com/track/click/31165340/help.openai.com?p=eyJzIjoibm1vUTJra2dWZ1NGNkVWczVhd1hwMEE4R20wIiwidiI6MSwicCI6IntcInVcIjozMTE2NTM0MCxcInZcIjoxLFwidXJsXCI6XCJodHRwczpcXFwvXFxcL2hlbHAub3BlbmFpLmNvbVxcXC9lblxcXC9hcnRpY2xlc1xcXC81MTEyNTk1LWJlc3QtcHJhY3RpY2VzLWZvci1hcGkta2V5LXNhZmV0eVwiLFwiaWRcIjpcImNlN2U1MzA1MzMyNTQ5ZjdhZmU5NGY4MTVhOTcwZWI1XCIsXCJ1cmxfaWRzXCI6W1wiNzI4ODA0ZmM5MzY4OWEyZTk2MDE2ZDNhYzYyZjhmZGY0MTc5MGJkOVwiXX0ifQ" target="_blank" style="-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;color:#10A37F;">best practices for API key safety</a>.
    </p>
    <p style="margin:0;margin-top:16px;">
      Best,<br>
      The OpenAI team
    </p>


  </td>
</tr>



        </table>
        <!--[if (gte mso 9)|(IE)]>
        </td>
        </tr>
        </table>
        <![endif]-->
      </td>
    </tr>
    <!-- end body block -->

    <!-- start footer -->
    <tr>
      <td align="center" style="padding:24px;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;">
        <!--[if (gte mso 9)|(IE)]>
        <table align="center" border="0" cellpadding="0" cellspacing="0" width="600">
        <tr>
        <td align="center" valign="top" width="600">
        <![endif]-->
        <table border="0" cellpadding="0" cellspacing="0" width="100%" style="max-width:560px;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;border-collapse:collapse ;">
            
  <tr>
  <td align="left" style="padding:4px 24px;font-size:14px;line-height:20px;color:#666;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;mso-table-rspace:0pt;mso-table-lspace:0pt;">
    <p style="margin: 0;">If you have any questions please contact us through our <a href="https://mandrillapp.com/track/click/31165340/help.openai.com?p=eyJzIjoidFcwQmh5c0tTbXI0OVROVFlNcGs1Z080d3AwIiwidiI6MSwicCI6IntcInVcIjozMTE2NTM0MCxcInZcIjoxLFwidXJsXCI6XCJodHRwczpcXFwvXFxcL2hlbHAub3BlbmFpLmNvbVxcXC9lblxcXC9cIixcImlkXCI6XCJjZTdlNTMwNTMzMjU0OWY3YWZlOTRmODE1YTk3MGViNVwiLFwidXJsX2lkc1wiOltcIjc3NTAwMDcwYzhjNTAzZTc2YTk4MTdmMGRhZjFiNTQ1ZGIyNTE1YThcIl19In0" style="-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%;font-family:Colfax, Helvetica, Arial, sans-serif;color:#10A37F;">help center</a></p>
  </td>
</tr>

        </table>
        <!--[if (gte mso 9)|(IE)]>
        </td>
        </tr>
        </table>
        <![endif]-->
      </td>
    </tr>
    <!-- end footer -->

  </table>
  <!-- end body -->
  <div class="debug-string" style="display: none; max-width: 0; max-height: 0; overflow: hidden; font-size: 1px; line-height: 1px; color: #ececf1; opacity: 0;">
      
  </div>

<img src="https://mandrillapp.com/track/open.php?u=31165340&id=ce7e5305332549f7afe94f815a970eb5" height="1" width="1" alt=""></body>
</html>
--_av-J7ojrq0M1BH4skdrgwiemw--
