# breadcrumb.js
Simple javascript library to create breadcrumbs in a web page based on the site url.
#
 -----------------------------------------------------------------------------
 
 
How to use:

1- Load the library file to your page.

	<script src="breadcrumb.js"></script>

2- Initialize breadcrumb.js by adding the next code in your page.

	<script>
		breadcrumb.init(
			container_id_to_render, 
			{
				stopLink: {}, 
				urlDivider: '', 
				divider: '', 
				groupCountainerTag: '', 
				containerTag: '', 
				cssStyleGroupContainer: '', 
				cssStyleTag: '', 
				cssStyle: '', 
			}
		);	
	</script>
 
 3- Enjoy it!
 
 -----------------------------------------------------------------------------
 
 Explanation:
 	
	breadcrumb.init(container_id_to_render, config)
 	
	container_id_to_render: Id of the breadcrumbs container.
		<div id="breadcrumb" class="any_class"></div>
	
	config: Configuration parameters.	
		stopLink: Array of actions that you don't want as links.
			stopLink: {
					edit: 'edit',
					show: 'show', 
				}
		
		urlDivider: Set the char where to split the url. By default takes "/".
			http://localhost/user/create
			
		divider: Divider to show between links in the breadcrumbs. By default takes " ".
			Home User Create
			
		groupCountainerTag: Cointainer to group all the links. Could be a list like <ol> or <ul>. Just write ul or ol, no need of <>.
		
		containerTag: Container of each link. Could be <li> if groupCountainerTag is a list tag. Just write li or span, no need of <>.
		
		cssStyleGroupContainer, cssStyleTag and cssStyle: Css styles for each container.
	
 -----------------------------------------------------------------------------
