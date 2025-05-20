<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>

<script type='text/javascript' src='https://service.force.com/embeddedservice/5.0/esw.min.js'></script>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
    console.log('Sonim devhub dev Chat');
		try {
      console.log('Sonim Try Block');
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
embeddedservice_bootstrap.settings.omitSandbox = true;
			embeddedservice_bootstrap.init(
				'00Dca000001GNMf',
				'EMEA_Web_Chat_SupportEmbedded',
				'https://sonimtech--dev.sandbox.my.site.com/ESWEMEAWebChatSupportE1732660542285',
				{
					scrt2URL: 'https://sonimtech--dev.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {

      console.log('Sonim Catch Block');
			console.error('Error loading Embedded Messaging: ', err);
		}
	};



</script>
<script type='text/javascript' src='https://sonimtech--dev.sandbox.my.site.com/ESWEMEAWebChatSupportE1732660542285/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
</body>
</html>
