![Screenshot1](https://dl.dropbox.com/u/339699/github/ASFBPostController.png)

ASFBPostController
==================

ASFBPostController provides photo posting function to Facebook.
You can easily integrate Facebook post function to you iOS app.

# Installation

1. Create your iOS facebook App (http://developers.facebook.com/).
2. Replace sample ID (1234567) with your Facebook App ID.

* ASFBPostController.m

	FB_APP_ID @"1234567"

* ASFBPost-Infor.plist

	URL types > Item 0 > URL Schemes > Item 0 > fb1234567

# Usage

	ASFBPostController *c = [[ASFBPostController alloc] init];
	c.thumbnailImage = [UIImage imageNamed:@"sample_thumb.jpg"];    
	c.originalImage = [UIImage imageNamed:@"sample.jpg"];

	UINavigationController *n = [[UINavigationController alloc] initWithRootViewController:c];
	n.modalPresentationStyle = UIModalPresentationFormSheet;
	[c release];
	
	[self presentModalViewController:n animated:YES];
	[n release];

License
==================
The ASFBPostController is licensed under the Apache License, Version 2.0 as same as the Facebook SDK.

Apache License
http://www.apache.org/licenses/LICENSE-2.0.html

Facebook iOS SDK
https://github.com/facebook/facebook-ios-sdk/

AppStair LLC
http://appstair.com
