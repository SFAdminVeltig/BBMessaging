<html>
	<style>
.vmiaw-prechat {
    padding: 18px 18px 14px;
    background: #fff;
    box-sizing: border-box;
    font-family: Georgia, "Times New Roman", Times, serif;
}

/* Header */
.vmiaw-prechat__header {
    text-align: center;
    margin-bottom: 18px;
}

.vmiaw-prechat__title {
    margin: 0;
    font-size: 36px;
    font-weight: 600;
    line-height: 1.1;
    color: #2d2929;
}

.vmiaw-prechat__subtitle {
    margin: 6px 0 0;
    font-size: 16px;
    color: #2d2929;
}

/* Fields */
.vmiaw-field {
    margin: 14px 0;
}

.vmiaw-label {
    display: block;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 13px;
    color: #2d2929;
    margin-bottom: 6px;
}

.vmiaw-required {
    color: #b00020;
    margin-right: 2px;
}

.vmiaw-input,
.vmiaw-select {
    width: 100%;
    height: 34px;
    box-sizing: border-box;
    border: 1px solid #b9b9b9;
    padding: 6px 10px;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 14px;
    outline: none;
    background: #fff;
}

.vmiaw-input:focus,
.vmiaw-select:focus {
    border-color: #7a7a7a;
}

.vmiaw-selectWrap {
    position: relative;
}

.vmiaw-select {
    appearance: none;
    -webkit-appearance: none;
    -moz-appearance: none;
    padding-right: 34px;
}

.vmiaw-selectCaret {
    position: absolute;
    right: 12px;
    top: 50%;
    width: 0;
    height: 0;
    pointer-events: none;
    transform: translateY(-30%);
    border-left: 6px solid transparent;
    border-right: 6px solid transparent;
    border-top: 7px solid #2d2929;
}

/* Help text */
.vmiaw-helptext {
    margin: 8px 0 0;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 12px;
    color: #2d2929;
}

/* Buttons */
.vmiaw-prechat__footer {
    margin-top: 14px;
}

.vmiaw-btn {
    width: 100%;
    height: 44px;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 16px;
    cursor: pointer;
    margin-top: 10px;
}

.vmiaw-btn--primary {
    background: #3f474f;      /* dark gray button */
    color: #fff;
    border: 1px solid #3f474f;
}

.vmiaw-btn--primary:hover {
    filter: brightness(0.95);
}

.vmiaw-btn--secondary {
    background: #fff;         /* white button */
    color: #000;
    border: 1px solid #000;
}

.vmiaw-btn--secondary:hover {
    background: #f6f6f6;
}

/* Recording text */
.vmiaw-recording {
    margin: 10px 0 0;
    text-align: center;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 10px;
    color: #2d2929;
    line-height: 1.25;
}

.vmiaw-recording a {
    color: #2d2929;
    text-decoration: underline;
}

/* Unavailable message */
.vmiaw-unavailable {
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 13px;
    color: #2d2929;
}

	</style>
  <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

		window.addEventListener("onEmbeddedMessagingReady", () => {            
			console.log( "Inside Prechat API!!" );
			embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( {'QueueName' : 'Boot Barn Messaging' } );
			});
			
			embeddedservice_bootstrap.init(
				'00DOt000002m0EL',
				'Boot_Barn_Messaging',
				'https://bootbarn--uat.sandbox.my.site.com/ESWBootBarnMessaging1770066084799',
				{
					scrt2URL: 'https://bootbarn--uat.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
  </script>
  <script type='text/javascript' src='https://bootbarn--uat.sandbox.my.site.com/ESWBootBarnMessaging1770066084799/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
</html>
