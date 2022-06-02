hugo serve <-- To run the local server  
hugo <-- Build for distribution  
hugo deploy <-- Push to S3.   
Checkout https://purnimakamath.com  

## Dear lord, why aren't my changes visible??
1. Did you invalidate cloudfront cache? If not wait 24 hours.    
2. Check your cloudfront origin - is it set to <domain name>-s3-website-<region> like url? Subfolders default paths dont work unless origin is setup like this. This should not change - but oh well you never know..   
3. Check the toml file, are you pushing to the right bucket?   
