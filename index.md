<html>
 <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			embeddedservice_bootstrap.settings.enableUserInputForConversationWithBot = false; // Prevent user from typing if bot hasn't responded.
			
			window.addEventListener("onEmbeddedMessagingReady", () => {            
				console.log( "Inside Prechat API!!" );
				embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( {'QueueName' : 'Boot Barn Messaging' } );
				});
	
			embeddedservice_bootstrap.init(
				'00DOt000011vrhd',
				'Boot_Barn_Messaging',
				'https://bootbarn--uat.sandbox.my.site.com/ESWBootBarnMessaging1774461017832',
				{
					scrt2URL: 'https://bootbarn--uat.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://bootbarn--uat.sandbox.my.site.com/ESWBootBarnMessaging1774461017832/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
<!--<script type='text/javascript' src='https://bootbarn.my.site.com/ESWBootBarnMessaging1774461017832/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>-->
</html>
