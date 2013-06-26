# Genesis Child Theme

1) Upload Genesis and Genesis-CT to your Web Server. Activate Genesis-CT

2) Genesis-CT uses a Less framework to customise the origional Genesis styling.

In the admin under "Genesis/Theme Settings" paste the following in the header. 

	<link rel="stylesheet/less" type="text/css" href="/wp-content/themes/genesis-ct/less/main.less" />
	<script type="text/javascript">
	    less = {
	        env: "development", 
	        async: false,       
	        fileAsync: false,  
	        poll: 1000,       
	        functions: {},      
	        dumpLineNumbers: "comments", 
	        relativeUrls: false,
	        rootpath: "http://gdfec.wdt3.co.uk/wp-content/themes/genesis-ct/"
	                           
	    };
	</script>
	<script src="/wp-content/themes/genesis-ct/less/less-1.3.3.min.js" type="text/javascript">

	less.watch();
	</script>

You can now enable watch mode while working, your styles will compile automatically on load.

3) Open the definitions.less file. Here you can adjust the colours, fonts and a few other choice properties.

4) Using coreStyles.less and themeStyles.less add any additional styling needed. 

5) When styling is finished. Compile the CSS (Newer folks use simpLESS). Then remove the code from "Genesis/Theme Settings".

