<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sonim Devhub Dev Chat</title>
</head>
<body>

<script type='text/javascript' src='https://service.force.com/embeddedservice/5.0/esw.min.js'></script>
<script type='text/javascript'>
  function initEmbeddedMessaging() {
    console.log('Sonim devhub dev Chat');
    try {
      console.log('Sonim Try Block');
      embeddedservice_bootstrap.settings.language = 'en_US'; // Set language
      embeddedservice_bootstrap.settings.omitSandbox = true;

      embeddedservice_bootstrap.init(
        '00Dca000001GNMf', // Salesforce Org ID
        'EMEA_Web_Chat_SupportEmbedded', // Embedded Messaging Deployment Name
        'https://sonimtech--dev.sandbox.my.site.com/ESWEMEAWebChatSupportE1732660542285', // Site Endpoint URL
        {
          scrt2URL: 'https://sonimtech--dev.sandbox.my.salesforce-scrt.com' // SCRT URL
        }
      );
    } catch (err) {
      console.log('Sonim Catch Block');
      console.error('Error loading Embedded Messaging: ', err);
    }
  }

  // Call the function on load
  window.addEventListener('load', initEmbeddedMessaging);
</script>

</body>
</html>

