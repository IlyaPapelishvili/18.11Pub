[["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/documentation-types@ko.md", ["Do", "Don't", "Do", "Don't", "Do", "Don't", "Do", "Don't", "Do", "Don't"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/formatting@de.md", ["Shortcodes", "Frontmatter", "Links", "orientation: default: landscape|portrait"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/formatting@fr.md", ["Shortcodes", "Frontmatter", "Images", "orientation: default: landscape|portrait"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/formatting@it.md", ["Frontmatter", "orientation: default: landscape|portrait"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/formatting@pl.md", ["orientation: default: landscape|portrait"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/formatting@pt_BR.md", ["Shortcodes", "Frontmatter", "Links", "orientation: default: landscape|portrait"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/formatting@ru.md", ["Shortcodes", "Frontmatter", "orientation: default: landscape|portrait"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/formatting@tr.md", ["orientation: default: landscape|portrait"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/index@es.md", ["Good first issues"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/index@id.md", ["Good first issues"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/index@ja.md", ["Good first issues"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/index@pt_BR.md", ["Good first issues"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/contribute-documentation/terminology@de.md", ["Definition"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/index@de.md", ["Helping with documentation", "Helping with translations"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/integrate-your-analytics-tools@tr.md", ["A new configuration json file ${vendorName}.json in the vendors folder including any options above and beyond the default, such as:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/translations@ja.md", ["Yes! Please translate this!", "Thanks for your interest, but the internal team or a volunteer is currently working on this document. You will be added as a reviewer before it goes live."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/vendor-contributions/ad-integration-guide@de.md", ["Ad Server ", "Data Management Platform (DMP) "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/vendor-contributions/ad-integration-guide@pl.md", ["Data Management Platform (DMP) "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/contribute/vendor-contributions/index@de.md", ["After deciding what level of contribution meets your use case, open a GitHub issue to start.", "Level 1 contributions leverage the feature logic of existing components. They load third party specific logic as custom JavaScript in a cross origin iframe. For example, many ad networks provide ads through the amp-ad component, but control how the rendering of ads through their own logic.", "amp-ad", "amp-analytics", "If you only need to add a tracking pixel with dynamic parameters to your tracking URL, check out amp-pixel. Be sure to document usage on your support pages for developers that may want to use your technology with AMP.", "amp-call-tracking", "If you are a technology provider for publishers or advertisers on the web, we invite you to add support to AMP! Your customers can continue to leverage your technology while working to achieve our vision of building a better web.", "There are 3 third party contribution levels. Levels are dependent on the amount of added logic:", "Third party logic: Code that is specific to the third party. This logic enables the component to leverage the third party service.", "Provide thorough documentation with code samples."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/custom-javascript@es.md", ["Web workers"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/custom-javascript@pt_BR.md", ["Web workers"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/interactivity/get-familiar@es.md", ["AMP boilerplate"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/interactivity/prereqs-setup@de.md", ["Step 1. Download the code", "Download the tutorial's starter code either as a ZIP file or via git:", "Start the development server with node.js:", "A basic knowledge of HTML, CSS, and JavaScript"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/interactivity/prereqs-setup@ko.md", ["Step 3. Run the development server"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/live_blog@ar.md", ["Every time a new item is added to the host document, the &lt;button update on=\"tap:my-live-list.update\"&gt; element shows a \"You have updates\" button which, when clicked, triggers the page to show the latest posts.", "Live blogs can grow and make the page too long. You can use the data-max-items-per-page attribute to specify how many items can be added to the live blog. If the number of items after an update exceeds data-max-items-per-page, the oldest updates exceeding this number are removed. For example, if the page currently has 9 items and data-max-items-per-page is set to 10, and 3 new items arrive in the latest update, the two oldest items are removed from the page with the latest update.", "All blog posts in the amp-live-list must be children of &lt;div items&gt;&lt;/div&gt;. By referring to each post as an item, every item must have a unique id and a data-sort-time.", "Now that you're familiar with the amp-live-list component, let's figure out how to implement a more complex live blog. Read on to learn more about how to implement pagination, and how deep linking works.", "Long blogs could use pagination to improve performance by limiting the number of blog items to display on a page. To implement pagination, in the amp-live-list component, add the &lt;div pagination&gt;&lt;/div&gt;, then insert any markup you need for pagination (for example, a page number or a link to the next and previous page).", "With pagination, the simple code we used earlier becomes:", "It's your responsibility to populate the navigation items correctly by updating the hosted page. For example, in the live blog sample we render the page via a server-side template and we use a query parameter to specify what the first blog item of the page should be. We limit the size of the page to 5 items, so if the server has generated more than 5 items, a user landing on the main page will see the \"Next\" element in the navigation area. Refer to amp-live-list for details.", "After the size of blog posts has exceeded the maximum number of items specified by data-max-items-per-page, the older blog items are displayed in the "Next" pages, for example on page 2. Given that the amp-live-list polls the server at intervals to see if there is any change in the items, there's no need to poll the server if the user isn't on the first page.", "When you publish a blog post, it's important to be able to deep link to the post to enable features like sharing. With amp-live-list, deep linking is possible by simply using the id of the blog item. For example, https://amp.dev/documentation/examples/news-publishing/live_blog/preview/index.html#post3 allows you to navigate directly to the blog post with the post3 id.", "AMP By Example uses a cookie to in the live blog sample to generate fresh content, so if it's the first time you are landing on the page, the post with id "post3" might not be available, in that case, you are redirected to the first post.", "Learn more from these resources:", "The amp-live-list component regularly polls the host document for new content and updates the user's browser as new items become available. This means that each time a new blog post needs to be added, the host document should be updated by the CMS to include the update in both the body and the metadata section of the page.", "This is what the initial code for the blog could look like:", "Let's look at this code:", "AMP BY Example's Live blog sample"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/live_blog@fr.md", ["Pagination ", "Deeplinking "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/live_blog@it.md", ["Overview of amp-live-list", "Implementation details", "Resources", "Pagination ", "Deeplinking ", "Live blogs are web pages that are updated frequently throughout an on-going event, such as a sporting event or an election. In AMP, you can implement a live blog by using the amp-live-list component.", "Every time a new item is added to the host document, the &lt;button update on=\"tap:my-live-list.update\"&gt; element shows a \"You have updates\" button which, when clicked, triggers the page to show the latest posts.", "Live blogs can grow and make the page too long. You can use the data-max-items-per-page attribute to specify how many items can be added to the live blog. If the number of items after an update exceeds data-max-items-per-page, the oldest updates exceeding this number are removed. For example, if the page currently has 9 items and data-max-items-per-page is set to 10, and 3 new items arrive in the latest update, the two oldest items are removed from the page with the latest update.", "All blog posts in the amp-live-list must be children of &lt;div items&gt;&lt;/div&gt;. By referring to each post as an item, every item must have a unique id and a data-sort-time.", "Now that you're familiar with the amp-live-list component, let's figure out how to implement a more complex live blog. Read on to learn more about how to implement pagination, and how deep linking works.", "Long blogs could use pagination to improve performance by limiting the number of blog items to display on a page. To implement pagination, in the amp-live-list component, add the &lt;div pagination&gt;&lt;/div&gt;, then insert any markup you need for pagination (for example, a page number or a link to the next and previous page).", "With pagination, the simple code we used earlier becomes:", "It's your responsibility to populate the navigation items correctly by updating the hosted page. For example, in the live blog sample we render the page via a server-side template and we use a query parameter to specify what the first blog item of the page should be. We limit the size of the page to 5 items, so if the server has generated more than 5 items, a user landing on the main page will see the \"Next\" element in the navigation area. Refer to amp-live-list for details.", "After the size of blog posts has exceeded the maximum number of items specified by data-max-items-per-page, the older blog items are displayed in the "Next" pages, for example on page 2. Given that the amp-live-list polls the server at intervals to see if there is any change in the items, there's no need to poll the server if the user isn't on the first page.", "This tutorial provides a short overview of the amp-live-list component and focuses on some implementation details for live blogs, like pagination and deep linking. We'll use AMP By Example's live blog sample to illustrate implementing live blogs in AMP.", "When you publish a blog post, it's important to be able to deep link to the post to enable features like sharing. With amp-live-list, deep linking is possible by simply using the id of the blog item. For example, https://amp.dev/documentation/examples/news-publishing/live_blog/preview/index.html#post3 allows you to navigate directly to the blog post with the post3 id.", "AMP By Example uses a cookie to in the live blog sample to generate fresh content, so if it's the first time you are landing on the page, the post with id "post3" might not be available, in that case, you are redirected to the first post.", "Learn more from these resources:", "The amp-live-list component regularly polls the host document for new content and updates the user's browser as new items become available. This means that each time a new blog post needs to be added, the host document should be updated by the CMS to include the update in both the body and the metadata section of the page.", "This is what the initial code for the blog could look like:", "Let's look at this code:", "amp-live-list reference documentation"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/live_blog@ko.md", ["AMP BY Example's Live blog sample"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/live_blog@pl.md", ["Overview of amp-live-list", "Implementation details", "Resources", "Pagination ", "Deeplinking ", "Live blogs are web pages that are updated frequently throughout an on-going event, such as a sporting event or an election. In AMP, you can implement a live blog by using the amp-live-list component.", "Every time a new item is added to the host document, the &lt;button update on=\"tap:my-live-list.update\"&gt; element shows a \"You have updates\" button which, when clicked, triggers the page to show the latest posts.", "Live blogs can grow and make the page too long. You can use the data-max-items-per-page attribute to specify how many items can be added to the live blog. If the number of items after an update exceeds data-max-items-per-page, the oldest updates exceeding this number are removed. For example, if the page currently has 9 items and data-max-items-per-page is set to 10, and 3 new items arrive in the latest update, the two oldest items are removed from the page with the latest update.", "All blog posts in the amp-live-list must be children of &lt;div items&gt;&lt;/div&gt;. By referring to each post as an item, every item must have a unique id and a data-sort-time.", "Now that you're familiar with the amp-live-list component, let's figure out how to implement a more complex live blog. Read on to learn more about how to implement pagination, and how deep linking works.", "Long blogs could use pagination to improve performance by limiting the number of blog items to display on a page. To implement pagination, in the amp-live-list component, add the &lt;div pagination&gt;&lt;/div&gt;, then insert any markup you need for pagination (for example, a page number or a link to the next and previous page).", "With pagination, the simple code we used earlier becomes:", "It's your responsibility to populate the navigation items correctly by updating the hosted page. For example, in the live blog sample we render the page via a server-side template and we use a query parameter to specify what the first blog item of the page should be. We limit the size of the page to 5 items, so if the server has generated more than 5 items, a user landing on the main page will see the \"Next\" element in the navigation area. Refer to amp-live-list for details.", "After the size of blog posts has exceeded the maximum number of items specified by data-max-items-per-page, the older blog items are displayed in the "Next" pages, for example on page 2. Given that the amp-live-list polls the server at intervals to see if there is any change in the items, there's no need to poll the server if the user isn't on the first page.", "This tutorial provides a short overview of the amp-live-list component and focuses on some implementation details for live blogs, like pagination and deep linking. We'll use AMP By Example's live blog sample to illustrate implementing live blogs in AMP.", "When you publish a blog post, it's important to be able to deep link to the post to enable features like sharing. With amp-live-list, deep linking is possible by simply using the id of the blog item. For example, https://amp.dev/documentation/examples/news-publishing/live_blog/preview/index.html#post3 allows you to navigate directly to the blog post with the post3 id.", "AMP By Example uses a cookie to in the live blog sample to generate fresh content, so if it's the first time you are landing on the page, the post with id "post3" might not be available, in that case, you are redirected to the first post.", "Learn more from these resources:", "The amp-live-list component regularly polls the host document for new content and updates the user's browser as new items become available. This means that each time a new blog post needs to be added, the host document should be updated by the CMS to include the update in both the body and the metadata section of the page.", "This is what the initial code for the blog could look like:", "Let's look at this code:", "The data-poll-interval attribute specifies how often polls should occur; if the host document is updated, the update should be available to the user after the next time interval.", "amp-live-list reference documentation", "AMP BY Example's Live blog sample"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/live_blog@ru.md", ["Overview of amp-live-list", "Implementation details", "Deeplinking ", "Live blogs can grow and make the page too long. You can use the data-max-items-per-page attribute to specify how many items can be added to the live blog. If the number of items after an update exceeds data-max-items-per-page, the oldest updates exceeding this number are removed. For example, if the page currently has 9 items and data-max-items-per-page is set to 10, and 3 new items arrive in the latest update, the two oldest items are removed from the page with the latest update.", "All blog posts in the amp-live-list must be children of &lt;div items&gt;&lt;/div&gt;. By referring to each post as an item, every item must have a unique id and a data-sort-time.", "It's your responsibility to populate the navigation items correctly by updating the hosted page. For example, in the live blog sample we render the page via a server-side template and we use a query parameter to specify what the first blog item of the page should be. We limit the size of the page to 5 items, so if the server has generated more than 5 items, a user landing on the main page will see the \"Next\" element in the navigation area. Refer to amp-live-list for details.", "After the size of blog posts has exceeded the maximum number of items specified by data-max-items-per-page, the older blog items are displayed in the "Next" pages, for example on page 2. Given that the amp-live-list polls the server at intervals to see if there is any change in the items, there's no need to poll the server if the user isn't on the first page.", "When you publish a blog post, it's important to be able to deep link to the post to enable features like sharing. With amp-live-list, deep linking is possible by simply using the id of the blog item. For example, https://amp.dev/documentation/examples/news-publishing/live_blog/preview/index.html#post3 allows you to navigate directly to the blog post with the post3 id.", "Let's look at this code:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@ar.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@de.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@es.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@fr.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@id.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@it.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@ja.md", ["Include the script", "Write the markup"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@ko.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@pl.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@pt_BR.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@ru.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@tr.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@vi.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/iframes@zh_CN.md", ["Learn how to display include media content in your pages, and how to use iframes to display advanced content outside of AMP's limitations."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/index@de.md", ["Video", "Audio", "Include a fallback, if the browser doesn't support HTML5 audio, for example:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/index@es.md", ["Video", "Audio", "Include a fallback, if the browser doesn't support HTML5 audio, for example:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/index@fr.md", ["Images", "Audio"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/index@id.md", ["Video", "Audio"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/index@it.md", ["Video", "Audio"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/index@tr.md", ["Video"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/index@vi.md", ["Video"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/third_party_components@pt_BR.md", ["Source:", "Preview:  ", "Source:", "Preview:  "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/media_iframes_3p/third_party_components@ru.md", ["Source:", "Preview:  ", "Source:", "Preview:  "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/monetization/index@de.md", ["AMP Real Time Config", "Sticky Ads", "Flying Carpet"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/monetization/index@id.md", ["Additional resources", "Demand &amp; pricing: get the right price for your ads", "Avoid heavy creatives per IAB guidelines.", "Avoid interstitials or other ad formats that cause the content to reflow on ad load.", "Place ads in your video content via supported players or amp-iframe to enable revenue on all types of content.", "Flying Carpet"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/monetization/index@it.md", ["Adding ads to your page", "Serving direct-sold AMPHTML ads", "Augmenting targeting data on ad requests", "Best practices", "Additional resources", "Step 1: Add the amp-ad script", "Innovation: Offer the most engaging ad products", "Step 2: Add the amp-ad tag to your AMP page", "Step 3: Specify the size of the ad unit", "Step 4: Set ad network parameters", "Step 5: (Optional) Specify a placeholder", "Step 6: (Optional) Specify a fallback", "Placement &amp; controls: optimize your ad placements", "Demand &amp; pricing: get the right price for your ads", "Ad types: Serve the best types of ads", "This guide provides instructions and best practices for displaying ads on your AMP pages.", "Depending on the ad network, you can choose to show a fallback element if no ad is available to serve. To specify a fallback, add a child element with the fallback attribute. Learn more in Placeholders &amp; fallbacks.", "Congratulations! You are now serving ads on your AMP page!", "You can learn more about RTC from this YouTube video:", "Or, learn more from these RTC resources:", "Here are some tips to maximize the effectiveness of ads on your AMP pages:", "Let's walk through the steps of adding the component so you can display ads on your AMP page.", "The amp-ad component is a custom ad extension to the AMP library. Under the hood of amp-ad is custom JavaScript that's carefully designed to optimize performance. To run the amp-ad component, you must add the required JavaScript for this component in the head section of your AMP page:", "In this example, we are adding an ad slot to serve ads from the a9 network:", "Place the same number of ads on AMP Pages as your non-AMP pages to generate maximum revenue per page.", "Place the first ad immediately below the first viewport (\"below the fold\") to provide an optimal user experience.", "Unless you're using advanced CSS or media queries, ensure your ad units are centered on the page to provide your users with an optimal mobile web experience.", "Enable multi-size ad requests on your AMP inventory to increase ad auction pressure and drive revenue.", "Sell ad units on your AMP pages across all sales channels, including direct and indirect to maximize competition for your inventory on AMP pages.", "Price your ad inventory on AMP pages similar to your inventory on non-AMP pages. Monitor performance and adjust pricing accordingly.", "Ensure all ad demand channels are competing for ad inventory on your AMP pages to drive up competition.", "Avoid heavy creatives per IAB guidelines.", "Avoid interstitials or other ad formats that cause the content to reflow on ad load.", "Optimize for viewability by setting the data-loading-strategy to prefer-viewability-over-views.", "Place ads in your video content via supported players or amp-iframe to enable revenue on all types of content.", "Implement ads on ancillary AMP pages to generate incremental revenue:", "... and more", "Implement new formats for direct sold ads to equip your sales team with high-impact, innovative ad products:"]],  

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@ar.md", ["Shaka Packager", "Web Story videos are always vertical (i.e., portrait view), with an expected aspect ratio of 16:9. Use the recommended resolution for the video streaming type:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@de.md", ["Shaka Packager", "Non-adaptive", "720 x 1280 px", "Adaptive", "720 x 1280 px540 x 960 px360 x 480 px", "Tool", "Animation", "Sponsored Story ", "Layout", "Video", "DOWNLOAD: \"Download\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@it.md", ["Shaka Packager", "Layout", "Video", "Video codec", "DOWNLOAD: \"Download\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@ja.md", ["Shaka Packager", "Custom text is allowed, but you will need to implement your own localization.", "The call to action button can be configured from a predefined set of choices:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@ko.md", ["Shaka Packager", "Call to action button text enum ", "Animation", "If support is needed for a new CTA button text enum, please open a GitHub issue."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@pl.md", ["Shaka Packager"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@pt_BR.md", ["Shaka Packager", "Sponsored Story ", "Layout", "Animation", "Video quality", "The CTA sits 32px from the bottom and is centered horizontally. It is 120px by 36px."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@ru.md", ["Shaka Packager"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@vi.md", ["Shaka Packager", "Video", "Video codec"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/story_ads_best_practices@zh_CN.md", ["Shaka Packager", "Video codec"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@ar.md", ["srcset"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@de.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@es.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@fr.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@id.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@it.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@ja.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@ko.md", ["srcset"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@pl.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@pt_BR.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@ru.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@tr.md", ["srcset"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@vi.md", ["srcset"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/art_direction@zh_CN.md", ["srcset", "sizes", "heights"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/control_layout@ar.md", ["The following values can be used in the layout attribute:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/control_layout@es.md", ["No", "No", "No", "No"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/responsive_design@ar.md", ["Scaling media for the page ", "Getty Images \"2016 in Focus\" ", "BRIT + CO's holiday gift guide", "The Guardian", "AMP Conf Workshop Codelab: Making beautiful AMPs"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/responsive_design@fr.md", ["Introduction", "Production", "Getty Images \"2016 in Focus\" ", "BRIT + CO's holiday gift guide", "The Guardian", "AMP Conf Workshop Codelab: Making beautiful AMPs"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/responsive_design@it.md", ["Getty Images \"2016 in Focus\" ", "BRIT + CO's holiday gift guide", "The Guardian"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/responsive_design@ru.md", ["Getty Images \"2016 in Focus\" ", "The Guardian"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/responsive_design@tr.md", ["Getty Images \"2016 in Focus\" ", "BRIT + CO's holiday gift guide", "The Guardian", "AMP Conf Workshop Codelab: Making beautiful AMPs"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/responsive_design@vi.md", ["Getty Images \"2016 in Focus\" ", "BRIT + CO's holiday gift guide", "The Guardian", "AMP Conf Workshop Codelab: Making beautiful AMPs"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/style_pages@de.md", ["When using preprocessors, pay special attention to what you include; load only what your pages use. For example, the head.html includes all required AMP mark-up and the inlined CSS from the *.scss source files. It also includes the custom element script for amp-youtube, among others, so that many pages across the site can include embedded youtube videos.", "To see how the above translates into formatted AMP HTML, view the source for any page in amp.dev. (In Chrome, right-click and View Page Source.)", "Like all web pages, AMP pages are styled with CSS, but you can't reference external stylesheets (with the exception of custom fonts). Also certain styles are disallowed due to performance implications.", "The following styles aren't allowed in AMP pages:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/develop/style_and_layout/style_pages@fr.md", ["Description", "Description"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/integrate/amp-in-pwa@fr.md", ["You'll still need to implement this step manually. After all, it's up to you how you present links to content in your navigation concept. A number of lists? A bunch of cards?", "Finally, when you want to display content after a user action, it's time to fetch the relevant AMP document and let Shadow AMP take over. First, implement a function to fetch the page, similar to this one:", "This code will work, and any number of callbacks added this way will indeed fire when AMP is available, but why?"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/integrate/amp-to-pwa@fr.md", ["In this case your canonical pages are your AMP pages: You're building your entire website with AMP, and simply use AMP as a library (fun fact: the very site you're reading this on is built this way). In this scenario, most links on your AMP pages will lead to other AMP pages.", "Then add the following somewhere within your &lt;body&gt; (modify to point to your actual Service Worker):"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/integrate/embed-stories@es.md", ["You may add multiple stories in the same &lt;amp-story-player&gt; element by defining multiple &lt;a&gt; tags. The player presents the second story's cover page after user's tap through the first.", "We recommend maintaining a 3:5 aspect ratio for the best user experience, but you may define any width and height."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/integrate/embed-stories@it.md", ["You may add multiple stories in the same &lt;amp-story-player&gt; element by defining multiple &lt;a&gt; tags. The player presents the second story's cover page after user's tap through the first.", "We recommend maintaining a 3:5 aspect ratio for the best user experience, but you may define any width and height."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/integrate/embed-stories@ko.md", ["You may add multiple stories in the same &lt;amp-story-player&gt; element by defining multiple &lt;a&gt; tags. The player presents the second story's cover page after user's tap through the first.", "We recommend maintaining a 3:5 aspect ratio for the best user experience, but you may define any width and height."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/integrate/embed-stories@vi.md", ["You may add multiple stories in the same &lt;amp-story-player&gt; element by defining multiple &lt;a&gt; tags. The player presents the second story's cover page after user's tap through the first.", "We recommend maintaining a 3:5 aspect ratio for the best user experience, but you may define any width and height."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/a4a_spec@pl.md", ["Boilerplate ", "CSS "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/a4a_spec@pt_BR.md", ["Boilerplate ", "CSS "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@ar.md", ["Fired when the form submission response is success.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "Target: amp-access "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@de.md", ["Event", "Event", "Event", "Event", "Event", "Event", "Fired when the form is invalid.", "Action", "Action", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "Syntax", "Event", "Event", "Event", "Event", "Event", "form ", "form ", "Target: amp-access ", "The actions for amp-access are dynamic depending on the structure of the AMP Access Configuration."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@es.md", ["scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@fr.md", ["Description", "Description", "Description", "Description", "Description", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "Action", "Description", "optoutOfCid", "Description", "Description", "Description", "Description", "Description", "Description", "form ", "form "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@id.md", ["Data", "Data", "Data", "Data", "Data", "Data", "Fired when the form is submitted.", "Fired when the form submission response is success.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "Data", "Data", "Data", "Data", "Target: AMP ", "Target: amp-access "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@it.md", ["Fired when the form is invalid.", "Hides the target element.", "Shows the target element. If an     autofocus element becomes visible as a     result, it gains focus.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "no", "no", "Event", "Target: AMP ", "Target: amp-access "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@ja.md", ["Fired when the form is submitted.", "Fired when the form submission response is success.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "form ", "form ", "Target: AMP ", "Target: amp-access "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@ko.md", ["Shows the target element. If an     autofocus element becomes visible as a     result, it gains focus.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@pl.md", ["scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "form ", "form "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@pt_BR.md", ["Fired when the form submission response is success.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "form ", "form "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@tr.md", ["Navigates current window to given URL, to the optional specified target if given (currenly only supporting _top and _blank ). The optional opener parameter can be specified when using a target of _blank to allow the newly opened page to access window.opener. Supports standard URL substitutions.", "Caveat: Using normal &lt;a&gt; links is recommended wherever possible since AMP.navigateTo is not recognized by web crawlers.", "Caveat: Using normal &lt;a&gt; links is recommended wherever possible since AMP.closeOrNavigateTo is not recognized by web crawlers.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "form ", "form "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@vi.md", ["Fired when the form is invalid.", "Hides the target element.", "Shows the target element. If an     autofocus element becomes visible as a     result, it gains focus.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "form "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-actions-and-events@zh_CN.md", ["Hides the target element.", "scrollTo(id=STRING, duration=INTEGER, position=STRING)", "optoutOfCid", "form "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/amp-cache-debugging@de.md", ["Symptom"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/amp-cache-debugging@fr.md", ["Solution"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/amp-cache-urls@de.md", ["URL Format"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/amp-cors-requests@fr.md", ["Access-Control-Allow-Origin: ", "Access-Control-Allow-Origin:  ", "Otherwise, process the request.", "URL https://example-com.cdn.ampproject.org/r/s/example.com/some/font.tff"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/amp-cors-requests@id.md", ["URL: https://amp.dev/documentation/guides-and-tutorials/start/create/", "Google AMP Cache subdomain: https://&lt;publisher's domain&gt;.cdn.ampproject.org (for example, https://nytimes-com.cdn.ampproject.org)", "URL https://example-com.cdn.ampproject.org/r/s/example.com/some/font.tff"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/amp-cors-requests@it.md", ["Access-Control-Allow-Origin:  ", "URL: https://amp.dev/documentation/guides-and-tutorials/start/create/", "Google AMP Cache Overview [/tip]", "URL https://example-com.cdn.ampproject.org/r/s/example.com/some/font.tff", "Access-Control-Allow-Origin: *"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/amp-cors-requests@ja.md", ["Access-Control-Allow-Origin: ", "Access-Control-Allow-Origin:  ", "URL: https://amp.dev/documentation/guides-and-tutorials/start/create/", "Google AMP Cache subdomain: https://&lt;publisher's domain&gt;.cdn.ampproject.org (for example, https://nytimes-com.cdn.ampproject.org)", "URL https://example-com.cdn.ampproject.org/r/s/example.com/some/font.tff", "Access-Control-Allow-Origin: *"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/amp-cors-requests@vi.md", ["URL: https://amp.dev/documentation/guides-and-tutorials/start/create/", "Google AMP Cache Overview [/tip]", "URL https://example-com.cdn.ampproject.org/r/s/example.com/some/font.tff", "Access-Control-Allow-Origin: *"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/how_amp_pages_are_cached@ar.md", ["Caching is a core part of the AMP ecosystem. Publishing a valid AMP document automatically opts it into cache delivery.", "Should you desire not to have your document cached, one option is to remove the amp attribute from the HTML tag. This makes the document technically invalid AMP, while not impacting the functionality of the document.", "By using the AMP format, you are making your content available to be cached by AMP Caches. There are a few ways that your AMP page can end up in an AMP Cache:", "Google AMP Cache URL example: https://foo-com.cdn.ampproject.org/c/s/foo.com/amp_document.html"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/how_amp_pages_are_cached@id.md", ["Google AMP Cache URL example: https://foo-com.cdn.ampproject.org/c/s/foo.com/amp_document.html"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/how_amp_pages_are_cached@pl.md", ["Google AMP Cache", "Bing AMP Cache"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-caches-and-cors/how_amp_pages_are_cached@ru.md", ["Google AMP Cache", "Bing AMP Cache"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-html-layout/index@de.md", ["Layout", "CSS \"display\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-html-layout/index@es.md", ["No", "No", "No", "No", "No", "No", "No", "No", "No", "No", "No", "No"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-html-layout/index@it.md", ["No", "No", "No", "No", "No", "No", "No", "No", "No", "No", "No", "No", "Layout"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-html-layout/index@ja.md", ["CSS \"display\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-html-layout/index@pt_BR.md", ["Layout", "CSS \"display\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-html-layout/index@tr.md", ["CSS \"display\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/amp-html-layout/index@vi.md", ["CSS \"display\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/common_attributes@ar.md", ["sizes", "Example:", "Most AMP elements support the media attribute. The value of media is a media query. If the query does not match, the element is not rendered and its resources and potentially its child resources will not be fetched. If the browser window changes size or orientation, the media queries are re-evaluated and elements are hidden and shown based on the new results.", "Example:", "Often used with: images, animations, videos, and ads", "Example:", "Often used with: lightboxes, sidebars, live lists, and forms", "Syntax:", "Example:", "Often used with: images, animations, videos, and ads", "Example:", "For more information, see Placeholders &amp; fallbacks.", "All AMP elements that support the responsive layout, also support the sizes attribute. The value of the AMP sizes attribute is a sizes expression that selects the defined size corresponding to the media query based on the current window size. Additionally, AMP sets an inline style for width on the element.", "Example:", "Often used with: images, animations, audio, and videos", "For more information, see Art direction with srcset, sizes &amp; heights.", "For some layouts, AMP components must have a width and height attribute that contains an integer pixel value.", "Example:", "For more information, see Layout &amp; Media queries and the Layout Spec.", "Example:", "Note: When the heights attribute is specified along with width and height, the layout is defaulted to responsive.", "Example:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/common_attributes@de.md", ["fallback", "heights", "layout", "media ", "noloading", "on", "placeholder", "sizes", "width and height", "Syntax:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/common_attributes@fr.md", ["fallback", "heights", "layout", "media ", "noloading", "on", "placeholder", "sizes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/common_attributes@it.md", ["fallback", "heights", "layout", "media ", "noloading", "on", "placeholder", "sizes", "width and height", "The value applies to the height, not the width of the element.", "Percent values are allowed. A percent value indicates the percent of the element's width. For example, a value of 80% indicates that the height of the element will be 80% of the element's width.", "AMP provides a set of layouts that specify how an AMP component behaves in the document layout. You can specify a layout for a component by adding the layout attribute with one of the supported layout values for the element (see the element's documentation for what values are supported).", "Example:", "Most AMP elements support the media attribute. The value of media is a media query. If the query does not match, the element is not rendered and its resources and potentially its child resources will not be fetched. If the browser window changes size or orientation, the media queries are re-evaluated and elements are hidden and shown based on the new results.", "Example:", "Often used with: images, animations, videos, and ads", "Example:", "The on attribute is used to install event handlers on elements. The events that are supported depend on the element.", "Often used with: lightboxes, sidebars, live lists, and forms", "Syntax:", "Example:", "The placeholder attribute indicates that the element marked with this attribute acts as a placeholder for the parent AMP element. The attribute can be placed on any HTML element that is a direct child of an AMP element that supports placeholders. By default, the placeholder is immediately shown for the AMP element, even if the AMP element's resources have not been downloaded or initialized. Once ready, the AMP element typically hides its placeholder and shows the content. The exact behavior with respect to the placeholder is up to the element's implementation.", "Often used with: images, animations, videos, and ads", "Example:", "For more information, see Placeholders &amp; fallbacks.", "All AMP elements that support the responsive layout, also support the sizes attribute. The value of the AMP sizes attribute is a sizes expression that selects the defined size corresponding to the media query based on the current window size. Additionally, AMP sets an inline style for width on the element.", "Example:", "Often used with: images, animations, audio, and videos", "For more information, see Art direction with srcset, sizes &amp; heights.", "For some layouts, AMP components must have a width and height attribute that contains an integer pixel value.", "Example:", "For more information, see Layout &amp; Media queries and the Layout Spec.", "Example:", "For more information, see Placeholders &amp; fallbacks.", "Note: When the heights attribute is specified along with width and height, the layout is defaulted to responsive."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/common_attributes@pl.md", ["fallback", "heights", "layout", "media ", "noloading", "on", "placeholder", "sizes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/common_attributes@ru.md", ["fallback", "heights", "layout", "media ", "noloading", "on", "placeholder", "sizes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/common_attributes@tr.md", ["fallback", "heights", "layout", "media ", "noloading", "on", "placeholder", "sizes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/common_attributes@vi.md", ["fallback", "heights", "layout", "media ", "noloading", "on", "placeholder", "sizes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-components@de.md", ["Layout ", "Element", "Element", "Element", "Layout"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-components@fr.md", ["Description", "Description", "Description"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-components@id.md", ["Media ", "Media"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-components@it.md", ["Layout ", "Layout"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-components@pl.md", ["Media ", "Element", "Element", "Element", "Media"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-components@pt_BR.md", ["Layout ", "Layout"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-css@fr.md", ["Pseudo-classes ", "Restrictions"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-css@pt_BR.md", ["Media features ", "Pseudo-classes "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-format@de.md", ["Feedback &amp; Support ", "AMP CLIENT_ID"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/email-spec/amp-email-format@fr.md", ["Validation ", "AMP CLIENT_ID"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/experimental@pt_BR.md", ["Origin trials"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/intro-to-amphtml-ads@ar.md", ["Carousel", "Video Parallax", "Lightbox", "TripleLift", "Dianomi", "Adzerk", "Google AdSense", "Celtra's Ad Creator", "Google Web Designer", "Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/intro-to-amphtml-ads@de.md", ["Video Parallax", "Lightbox", "FAQs", "TripleLift", "Dianomi", "Adzerk", "Google AdSense", "Celtra's Ad Creator", "Google Web Designer", "Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/intro-to-amphtml-ads@fr.md", ["Carousel", "Video Parallax", "Lightbox", "Formats", "DoubleClick for Publishers", "TripleLift", "Dianomi", "Adzerk", "Google AdSense", "Google Web Designer", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/intro-to-amphtml-ads@id.md", ["Lightbox", "Yes. See amp-ad-exit.", "Why are AMPHTML ads better than traditional ads?", "DoubleClick for Publishers", "TripleLift", "Dianomi", "Adzerk", "Google AdSense", "Celtra's Ad Creator", "Google Web Designer", "Adobe Animate (coming soon)", "Celtra's Ad Creator", "Google Web Designer", "Adobe Animate (coming soon)", "Use the AMP validator for one-off testing.", "Partner with Cloudflare and use their public validator end point.", "Stack Overflow is our recommended way to find answers to questions about AMP; since members of the AMP Project community regularly monitor Stack Overflow you will probably receive the fastest response to your questions there.", "Join the Slack #a4a-discuss channel for solutions and answers.", "If you encounter a bug in AMP or have a feature request for AMP, see Reporting issues with AMP for information on filing an issue."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/intro-to-amphtml-ads@it.md", ["Video Parallax", "Lightbox", "Why are AMPHTML ads better than traditional ads?", "DoubleClick for Publishers", "TripleLift", "Dianomi", "Adzerk", "Google AdSense", "Celtra's Ad Creator", "Google Web Designer", "Adobe Animate (coming soon)", "Celtra's Ad Creator", "Google Web Designer", "Adobe Animate (coming soon)", "Use the AMP validator for one-off testing.", "Partner with Cloudflare and use their public validator end point.", "Stack Overflow is our recommended way to find answers to questions about AMP; since members of the AMP Project community regularly monitor Stack Overflow you will probably receive the fastest response to your questions there.", "Join the Slack #a4a-discuss channel for solutions and answers.", "If you encounter a bug in AMP or have a feature request for AMP, see Reporting issues with AMP for information on filing an issue."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/intro-to-amphtml-ads@pl.md", ["Lightbox", "DoubleClick for Publishers", "TripleLift", "Dianomi", "Adzerk", "Google AdSense", "Celtra's Ad Creator", "Google Web Designer", "Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/intro-to-amphtml-ads@ru.md", ["Lightbox", "DoubleClick for Publishers", "TripleLift", "Dianomi", "Adzerk", "Google AdSense", "Google Web Designer", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/intro-to-amphtml-ads@vi.md", ["Video Parallax", "Lightbox", "DoubleClick for Publishers", "TripleLift", "Dianomi", "Adzerk", "Google AdSense", "Celtra's Ad Creator", "Google Web Designer", "Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/spec/amphtml@de.md", ["frame", "frameset", "object", "param", "applet", "embed", "form", "button", "Status in AMP HTML", "link", "meta", "svg", "script", "noscript", "base", "img", "picture", "video", "audio", "iframe", "SVG ", "Stylesheets ", "HTML Tags ", "IDs ", "Links ", "layout, width, height, media, placeholder, fallback ", "URL ", "URL ", "@font-face, @keyframes, @media, @page, @supports.", "Fonts.com: https://fast.fonts.net", "Google Fonts: https://fonts.googleapis.com", "Font Awesome: https://maxcdn.bootstrapcdn.com, https://use.fontawesome.com", "\"style\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/spec/amphtml@es.md", ["frame", "frameset", "object", "param", "applet", "embed", "form", "input elements", "button", "link", "meta", "svg", "script", "noscript", "base", "img", "picture", "video", "audio", "iframe", "SVG ", "@-rules ", "layout, width, height, media, placeholder, fallback ", "URL ", "URL ", "@font-face, @keyframes, @media, @page, @supports.", "Fonts.com: https://fast.fonts.net", "Google Fonts: https://fonts.googleapis.com", "Font Awesome: https://maxcdn.bootstrapcdn.com, https://use.fontawesome.com", "\"style\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/spec/amphtml@fr.md", ["frame", "frameset", "object", "param", "applet", "embed", "form", "input elements", "button", "link", "meta", "svg", "script", "noscript", "base", "img", "picture", "video", "audio", "iframe", "Performance ", "SVG ", "Classes ", "Important ", "layout, width, height, media, placeholder, fallback ", "URL ", "URL ", "@font-face, @keyframes, @media, @page, @supports.", "Example: on=\"tap:fooId.showLightbox\"", "Fonts.com: https://fast.fonts.net", "Google Fonts: https://fonts.googleapis.com", "Font Awesome: https://maxcdn.bootstrapcdn.com, https://use.fontawesome.com", "\"style\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/spec/amphtml@id.md", ["frame", "frameset", "object", "param", "applet", "embed", "form", "button", "Tag", "link", "meta", "svg", "script", "noscript", "base", "img", "picture", "video", "audio", "iframe", "SVG ", "Metadata ", "layout, width, height, media, placeholder, fallback ", "URL ", "URL ", "@font-face, @keyframes, @media, @page, @supports.", "Fonts.com: https://fast.fonts.net", "Google Fonts: https://fonts.googleapis.com", "Font Awesome: https://maxcdn.bootstrapcdn.com, https://use.fontawesome.com", "\"style\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/spec/amphtml@it.md", ["frame", "frameset", "object", "param", "applet", "embed", "form", "input elements", "button", "Tag", "link", "meta", "svg", "script", "noscript", "base", "img", "picture", "video", "audio", "iframe", "SVG ", "@-rules ", "Important ", "layout, width, height, media, placeholder, fallback ", "URL ", "URL ", "@font-face, @keyframes, @media, @page, @supports.", "Fonts.com: https://fast.fonts.net", "Google Fonts: https://fonts.googleapis.com", "Font Awesome: https://maxcdn.bootstrapcdn.com, https://use.fontawesome.com", "Typekit: https://use.typekit.net/kitId.css (replace kitId accordingly)", "\"style\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/spec/amphtml@ja.md", ["frame", "frameset", "object", "param", "applet", "embed", "form", "input elements", "button", "link", "meta", "svg", "script", "noscript", "base", "img", "picture", "video", "audio", "iframe", "SVG ", "Important ", "URL ", "URL ", "Fonts.com: https://fast.fonts.net", "Google Fonts: https://fonts.googleapis.com", "\"style\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/spec/amphtml@vi.md", ["frame", "frameset", "object", "param", "applet", "embed", "form", "button", "link", "meta", "svg", "script", "noscript", "base", "img", "picture", "video", "audio", "iframe", "SVG ", "layout, width, height, media, placeholder, fallback ", "URL ", "URL ", "@font-face, @keyframes, @media, @page, @supports.", "Fonts.com: https://fast.fonts.net", "Google Fonts: https://fonts.googleapis.com", "Font Awesome: https://maxcdn.bootstrapcdn.com, https://use.fontawesome.com", "\"style\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/spec/amphtml@zh_CN.md", ["frame", "frameset", "object", "param", "applet", "embed", "form", "button", "link", "meta", "svg", "script", "noscript", "base", "img", "picture", "video", "audio", "iframe", "SVG ", "Font Awesome: https://maxcdn.bootstrapcdn.com, https://use.fontawesome.com", "\"style\""]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/validation-workflow/validate_emails@de.md", ["Installation"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/validation-workflow/validate_emails@fr.md", ["Installation"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/validation-workflow/validate_emails@id.md", ["AMP playground"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/validation-workflow/validate_emails@tr.md", ["AMP playground"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/validation-workflow/validation_errors@pt_BR.md", ["\"The mandatory text (CDATA) inside tag '%1' is missing or incorrect.\"", "\"The text (CDATA) inside tag '%1' matches '%2', which is disallowed.\"", "\"The property '%1' in attribute '%2' in tag '%3' is disallowed.\"", "\"The property '%1' in attribute '%2' in tag '%3' is set to '%4', which is invalid.\"", "\"Missing URL for attribute '%1' in tag '%2'.\"", "\"Malformed URL '%3' for attribute '%1' in tag '%2'\"", "Invalid URL protocol '%3:' for attribute '%1' in tag '%2'.", "\"The property '%1' is missing from attribute '%2' in tag '%3'.\"", "\"Mutually exclusive attributes encountered in tag '%1' - pick one of %2.\"", "\"The parent tag of tag '%1' is '%2', but it can only be '%3'.\"", "\"The tag '%1' may not appear as a descendant of tag '%2'.\"", "\"The tag '%1' may only appear as a descendant of tag '%2'.\"", "\"The tag '%1' may only appear as a descendant of tag '%2'. Did you mean '%3'?\"", "\"The tag '%1' appears more than once in the document.\"", "\"The author stylesheet specified in tag 'style' is too long - we saw %1 bytes whereas the limit is %2 bytes.\"", "\"CSS syntax error in tag '%1' - %2.\"", "\"CSS syntax error in tag '%1' - saw invalid at rule '%2'.\"", "\"The implied layout '%1' is not supported by tag '%2'.\"", "\"The attribute '%1' in tag '%2' is disallowed by implied layout '%3'.\"", "\"The specified layout '%1' is not supported by tag '%2'.\"", "\"The attribute '%1' in tag '%2' is disallowed by implied layout '%3'.\"", "\"Invalid value '%1' for attribute '%2' in tag '%3' - for layout '%4', set the attribute '%2' to value '%5'.\"", "\"Inconsistent units for width and height in tag '%1' - width is specified in '%2' whereas height is specified in '%3'.\"", "\"Mustache template syntax in attribute name '%1' in tag '%2'.\"", "\"The attribute '%1' in tag '%2' is set to '%3', which contains unescaped Mustache template syntax.\"", "\"The attribute '%1' in tag '%2' is set to '%3', which contains a Mustache template partial.\"", "No error message defined as yet (no deprecated tags).", "\"The attribute '%1' in tag '%2' is deprecated - use '%3' instead.\"", "\"The mandatory tag '%1' is missing or incorrect.\"", "\"The '%1' tag is missing or incorrect, but required by '%2'.\"", "\"The tag '%1' is disallowed.\"", "\"Custom JavaScript is not allowed.\"", "\"The mandatory attribute '%1' is missing in tag '%2'.\"", "\"The attribute '%1' in tag '%2' is set to the invalid value '%3'.\"", "\"The attribute '%1' may not appear in tag '%2'.\"", "\"Mandatory style boilerplate (js enabled)\"", "\"Disallowed @page in CSS\" [filter formats=\"websites, stories, ads\"]", "\"Disallowed @viewport in CSS\" [/filter]", "\"Mandatory style boilerplate (noscript)\"", "\"Disallowed -amp- CSS class name prefix\"", "\"Disallowed !important attribute in CSS\"", "\"Disallowed @charset in CSS\"", "\"Disallowed @import in CSS\"", "\"Disallowed @namespace in CSS\"", "\"Disallowed @supports in CSS\"", "\"Disallowed @document in CSS\"", "\"\\\\.i?-amp-\" (\"CSS -amp- class name prefix\")"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/webstory_technical_details@de.md", ["Video"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/webstory_technical_details@es.md", ["Video"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/webstory_technical_details@fr.md", ["AMP Valid"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/webstory_technical_details@id.md", ["AMP Valid", "Video"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/webstory_technical_details@it.md", ["Video"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/webstory_technical_details@tr.md", ["Video"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/learn/webstory_technical_details@vi.md", ["Video"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-as-pwa@fr.md", ["Installing the AMP Service Worker"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-managing-user-state@fr.md", ["IMPORTANT:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/explainer@id.md", ["⁣**2. Inline AMP-internal CSS styles: ** the AMP-boilerplate code is replaced by the AMP-runtime CSS styles: &lt;style amp-runtime&gt;...&lt;/style&gt;. For non-server-side rendered documents, AMP adds these styles at runtime. However, server-side-rendered AMP pages require these for the AMP layouts to work before AMP has been loaded. To avoid potential version conflicts, at runtime, AMP will check if the version specified in i-amphtml-version=\"011905222334000\" differs from the current AMP version and will update the CSS with the latest version if not."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/explainer@vi.md", ["⁣**2. Inline AMP-internal CSS styles: ** the AMP-boilerplate code is replaced by the AMP-runtime CSS styles: &lt;style amp-runtime&gt;...&lt;/style&gt;. For non-server-side rendered documents, AMP adds these styles at runtime. However, server-side-rendered AMP pages require these for the AMP layouts to work before AMP has been loaded. To avoid potential version conflicts, at runtime, AMP will check if the version specified in i-amphtml-version=\"011905222334000\" differs from the current AMP version and will update the CSS with the latest version if not."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/index@ar.md", ["Add yours?", "AMP Toolbox for PHP: a PHP based library for producing optimized AMP. The implementation is maintained by the AMP team.", "Netlify AMP Optimizer Plugin", "Add yours?"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/index@fr.md", ["Add yours?", "AMP Toolbox for PHP: a PHP based library for producing optimized AMP. The implementation is maintained by the AMP team.", "Netlify AMP Optimizer Plugin", "Add yours?"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/index@ja.md", ["Add yours?", "AMP Toolbox for PHP: a PHP based library for producing optimized AMP. The implementation is maintained by the AMP team.", "Netlify AMP Optimizer Plugin", "Add yours?"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/index@ko.md", ["Add yours?", "AMP Toolbox for PHP: a PHP based library for producing optimized AMP. The implementation is maintained by the AMP team.", "Netlify AMP Optimizer Plugin", "Add yours?"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/index@zh_CN.md", ["Add yours?", "AMP Toolbox for PHP: a PHP based library for producing optimized AMP. The implementation is maintained by the AMP team.", "Netlify AMP Optimizer Plugin", "Add yours?"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/node-amp-optimizer@de.md", ["Setup"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp-optimizer-guide/node-amp-optimizer@fr.md", ["Configuration"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp_to_pwa@ar.md", ["You should be able to view the landing page for Lyrical Lyghtning, the Mobile Music Magic festival. It has one link on the homepage to view the schedule and which stage the bands are on."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp_to_pwa@de.md", ["You should be able to view the landing page for Lyrical Lyghtning, the Mobile Music Magic festival. It has one link on the homepage to view the schedule and which stage the bands are on."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp_to_pwa@es.md", ["The &lt;amp-install-serviceworker&gt; installs the service worker by creating an iframe and running the data-iframe-src file. Create the install-sw.html file and add the following code:", "You should be able to view the landing page for Lyrical Lyghtning, the Mobile Music Magic festival. It has one link on the homepage to view the schedule and which stage the bands are on."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp_to_pwa@ja.md", ["The &lt;amp-install-serviceworker&gt; installs the service worker by creating an iframe and running the data-iframe-src file. Create the install-sw.html file and add the following code:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/amp_to_pwa@tr.md", ["Prefetch links "]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@de.md", ["My homepage", "Trigger", "my user", "Trigger", "This allows you to do things like vary the configuration based on a specific request. If you as the publisher have control over the remote file, you can do any server-side processing necessary to construct the configuration data.", "The first step to loading remote configurations is to include the config attribute in the amp-analytics tag:", "Include the transport attribute in your configuration only if you want to limit the transport options, otherwise, you may stop requests.", "In the example below, beacon and xhrpost are set to false, so they will not be used even though they have higher precedence than image. If the client's user agent supports the image method, then it will be used; otherwise, no request gets sent.", "AMP populates variables with values in an order of precedence:", "In this example, there's a remote configuration, variables defined at the top-level, in triggers, and at the platform level:", "When the same var is defined in multiple locations, the variable order of precedence sets its value once. Thus, if the remote configuration defined account as UA-XXXXX-Y in the example above, the values of various vars will be as follows:", "AMP is designed to support two common patterns of data collection:", "To send analytics data to an analytics provider, include the type attribute in the amp-analytics tag and set its value to the appropriate vendor, as defind in the Analytics Vendors list.", "For example: &lt;amp-analytics type=\"googleanalytics\"&gt; sends analytics data to the third-party analytics provider, Google Analytics. To send data to a publisher-owned endpoint, simply don't include the type attribute; the analytics data is sent to the defined endpoints for each request.", "Analytics vendor configurations are a quick way to get started with amp-analytics. You should consult your vendor's documentation and help resources for further guidance. As previously mentioned, the list of vendors who've already integrated with AMP, as well as links to their specific documentation can be found in the Analytics Vendors list.", "Ingestion by a publisher-owned endpoint for in-house analytics systems.", "Ingestion by a vendor-owned endpoint for interoperability with a vendor solution (for example, Adobe Analytics, Chartbeat, Google Analytics)."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@es.md", ["My homepage", "my user"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@fr.md", ["Description", "Description", "My homepage", "my user"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@id.md", ["Platform", "AMP is designed to support two common patterns of data collection:", "Ingestion by a vendor-owned endpoint for interoperability with a vendor solution (for example, Adobe Analytics, Chartbeat, Google Analytics)."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@it.md", ["Trigger Config", "My homepage", "Trigger", "my user", "Trigger", "In this example, there's a remote configuration, variables defined at the top-level, in triggers, and at the platform level:", "When the same var is defined in multiple locations, the variable order of precedence sets its value once. Thus, if the remote configuration defined account as UA-XXXXX-Y in the example above, the values of various vars will be as follows:", "AMP is designed to support two common patterns of data collection:", "To send analytics data to an analytics provider, include the type attribute in the amp-analytics tag and set its value to the appropriate vendor, as defind in the Analytics Vendors list.", "For example: &lt;amp-analytics type=\"googleanalytics\"&gt; sends analytics data to the third-party analytics provider, Google Analytics. To send data to a publisher-owned endpoint, simply don't include the type attribute; the analytics data is sent to the defined endpoints for each request.", "Analytics vendor configurations are a quick way to get started with amp-analytics. You should consult your vendor's documentation and help resources for further guidance. As previously mentioned, the list of vendors who've already integrated with AMP, as well as links to their specific documentation can be found in the Analytics Vendors list.", "If you're an analytics vendor, learn more about integrating your own analytics configuration into AMP HTML.", "Ingestion by a publisher-owned endpoint for in-house analytics systems.", "Ingestion by a vendor-owned endpoint for interoperability with a vendor solution (for example, Adobe Analytics, Chartbeat, Google Analytics)."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@ja.md", ["My homepage", "my user"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@ko.md", ["Ingestion by a publisher-owned endpoint for in-house analytics systems.", "Ingestion by a vendor-owned endpoint for interoperability with a vendor solution (for example, Adobe Analytics, Chartbeat, Google Analytics)."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@pl.md", ["My homepage", "my user", "When the same var is defined in multiple locations, the variable order of precedence sets its value once. Thus, if the remote configuration defined account as UA-XXXXX-Y in the example above, the values of various vars will be as follows:", "AMP is designed to support two common patterns of data collection:", "To send analytics data to an analytics provider, include the type attribute in the amp-analytics tag and set its value to the appropriate vendor, as defind in the Analytics Vendors list.", "For example: &lt;amp-analytics type=\"googleanalytics\"&gt; sends analytics data to the third-party analytics provider, Google Analytics. To send data to a publisher-owned endpoint, simply don't include the type attribute; the analytics data is sent to the defined endpoints for each request.", "Analytics vendor configurations are a quick way to get started with amp-analytics. You should consult your vendor's documentation and help resources for further guidance. As previously mentioned, the list of vendors who've already integrated with AMP, as well as links to their specific documentation can be found in the Analytics Vendors list.", "If you're an analytics vendor, learn more about integrating your own analytics configuration into AMP HTML.", "Ingestion by a vendor-owned endpoint for interoperability with a vendor solution (for example, Adobe Analytics, Chartbeat, Google Analytics)."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@pt_BR.md", ["Platform", "My homepage", "Trigger", "Remote configuration", "my user", "Trigger", "Value", "Defined By"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@tr.md", ["Platform", "My homepage", "my user"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@vi.md", ["Requests, triggers &amp; transports ", "AMP is designed to support two common patterns of data collection:", "To send analytics data to an analytics provider, include the type attribute in the amp-analytics tag and set its value to the appropriate vendor, as defind in the Analytics Vendors list.", "For example: &lt;amp-analytics type=\"googleanalytics\"&gt; sends analytics data to the third-party analytics provider, Google Analytics. To send data to a publisher-owned endpoint, simply don't include the type attribute; the analytics data is sent to the defined endpoints for each request.", "If you're an analytics vendor, learn more about integrating your own analytics configuration into AMP HTML."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/deep_dive_analytics@zh_CN.md", ["My homepage", "my user"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/index@de.md", ["Learn more: Continue to learn about analytics with Analytics: the Basics."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/configure-analytics/use_cases@es.md", ["The following example uses the selector attribute of the trigger to send an event when a particular social button is clicked (see also AMP social interactions tracking in Google Analytics):", "Learn how to track page views using amp-pixel and amp-analytics.", "Send pageview data to a specified URL using amp-pixel:", "Send pageview data to a specified URL using amp-analytics:", "Send pageview data to Google Analytics (see also Page tracking in Google Analytics):", "Learn how to track page clicks using amp-analytics, sending event data to a specified URL, and to Google Analytics.", "The following example uses the selector attribute to send a click event to the specified URL everytime a user clicks on a link (&lt;a href&gt;):"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/discovery@zh_CN.md", ["Learn how to Structure your content to appear in Google Search rich results (e.g., top stories carousel, recipe cards, etc.)."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/optimize_amp@ar.md", "If you are using Google fonts, or any other font provider with unknown font URLs, preconnect the respective font server:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/optimize_amp@pl.md", ["Use preconnect to speedup the connection to other origin where the full resource URL is not known ahead of time, for example, when using Google Fonts:", "Load the AMP runtime:", "Specify the &lt;script&gt; tags for render-delaying extensions (e.g., amp-experiment amp-dynamic-css-classes and amp-story", "Finally, specify the AMP boilerplate code. By putting the boilerplate code last, it prevents custom styles from accidentally overriding the boilerplate css rules.]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/optimize_amp@pt_BR.md", "Use HTTP Caching"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@ar.md", ["AMP Linter", "Cloudflare AMP Real URL", "iframes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@de.md", ["The AMP Validator ", "AMP Linter", "AMP Tools", "CORS in AMP", "Signed HTTP Exchanges", "Cloudflare AMP Real URL", "Signed exchanges for better AMP URLs and easier analytics (AMP Conf '19)", "iframes", "So your AMP test doesn't perform — now what?", "Cache vs. non-cache analysis", "Measuring success: What's new in AMP analytics &amp; experiments (AMP Conf '19)", "Signed exchanges for better AMP URLs and easier analytics (AMP Conf '19)"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@es.md", ["AMP Linter", "videos", "iframes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@fr.md", ["AMP Linter", "images", "iframes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@ja.md", ["Google AMP Tester", "AMP Linter", "Signed HTTP Exchanges", "Cloudflare AMP Real URL", "So your AMP test doesn't perform — now what?", "Cache vs. non-cache analysis", "Measuring user journeys across the AMP Cache and your website", "Signed exchanges for better AMP URLs and easier analytics (AMP Conf '19)"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@pl.md", ["Google AMP Tester", "AMP Linter"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@pt_BR.md", ["Google AMP Tester", "AMP Linter", "AMP Tools", "Cloudflare AMP Real URL", "Signed exchanges for better AMP URLs and easier analytics (AMP Conf '19)", "iframes", "AMP on Google, Google AMP Cache", "Measuring success: What's new in AMP analytics &amp; experiments (AMP Conf '19)", "Signed exchanges for better AMP URLs and easier analytics (AMP Conf '19)"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@ru.md", ["AMP Linter", "Cloudflare AMP Real URL"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@tr.md", ["Google AMP Tester", "AMP Linter", "iframes"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@vi.md", ["Google AMP Tester", "AMP Linter"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/publishing_checklist@zh_CN.md", ["AMP Linter"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/optimize-measure/signed-exchange@fr.md", ["Configuration", "Installation", "Installation"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/add_advanced/adding_carousels@de.md", ["Refresh your page and you should see a carousel:", "Next, add the loop attribute. Refresh the page and try swiping to the left immediately. The carousel loops endlessly."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/add_advanced/adding_components@de.md", ["Tweets"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/add_advanced/tracking_data@ar.md", ["Analytics platforms are commonly integrated into websites through inline JavaScript snippets and function calls, which trigger events that are sent back to the analytics system. AMP provides a flexible JSON configuration syntax to replicate this process for several analytics partners."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/add_advanced/tracking_data@de.md", ["Analytics platforms are commonly integrated into websites through inline JavaScript snippets and function calls, which trigger events that are sent back to the analytics system. AMP provides a flexible JSON configuration syntax to replicate this process for several analytics partners."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/converting/resolving-errors@es.md", ["What is DOM reflow?"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@ar.md", ["Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@de.md", ["Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@es.md", ["Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@fr.md", ["Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@id.md", ["Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@it.md", ["Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@ja.md", ["Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@ko.md", ["Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@pl.md", ["Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@pt_BR.md", ["Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@ru.md", ["Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@tr.md", ["Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@vi.md", ["Celtra's Ad Creator", "Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/create_amphtml_ad/index@zh_CN.md", ["Google Web Designer"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email-inspiration@fr.md", ["Collaboration"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@ar.md", ["Verizon Media (Yahoo Mail)", "Verizon Media Privacy Policy - US"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@de.md", ["Verizon Media (Yahoo Mail)", "Verizon Media Privacy Policy - US"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@es.md", ["Verizon Media (Yahoo Mail)"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@fr.md", ["Confirmation", "Verizon Media (Yahoo Mail)"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@id.md", ["Verizon Media (Yahoo Mail)"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@ja.md", ["Verizon Media (Yahoo Mail)", "Verizon Media Privacy Policy - US"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@ko.md", ["Verizon Media (Yahoo Mail)"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@pt_BR.md", ["GooglePrivacy &amp; Terms", "Mail.ru", "Verizon Media (Yahoo Mail)", "Non-Russian based users", "Russian based users", "Verizon Media Privacy Policy - US"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@ru.md", ["Verizon Media (Yahoo Mail)"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@vi.md", ["GooglePrivacy &amp; Terms", "Mail.ru", "Verizon Media (Yahoo Mail)", "Non-Russian based users", "Russian based users", "Verizon Media Privacy Policy - US"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/email_sender_distribution@zh_CN.md", ["GooglePrivacy &amp; Terms", "Mail.ru", "Verizon Media (Yahoo Mail)", "Non-Russian based users", "Russian based users", "Verizon Media Privacy Policy - US"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/add_more_pages@ar.md", ["Demonstrates how to arrange text and display a screen-filling video for the page.", "Our \"Joy of Pets\" story is nearly complete. We'll use animations in our last page to bring all the pets together."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/add_more_pages@fr.md", ["Demonstrates how to arrange text and display a screen-filling video for the page.", "Our \"Joy of Pets\" story is nearly complete. We'll use animations in our last page to bring all the pets together."]],  

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/animating_elements@zh_CN.md", ["It looks great but everything is static! Let's animate!"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/congratulations@ar.md", ["You have successfully completed your first Web Story using AMP!", "Learn more about Web Stories and AMP from these resources:", "Create a multi-page Web Story by using the amp-story component"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/congratulations@fr.md", ["You have successfully completed your first Web Story using AMP!", "Learn more about Web Stories and AMP from these resources:", "Create a multi-page Web Story by using the amp-story component"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@ar.md", ["small", "landscape", "portrait", "cta-link"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@de.md", ["heading", "small", "landscape", "portrait", "cta-link"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@fr.md", ["heading", "small", "landscape", "portrait", "cta-link", "Type", "Description", "There are various components that you can use to display related content and links; each component is specified with a type attribute. Let's look at the available components:", "There's more to learn about the bookend component. For details, see the amp-story reference documentation.", "The information on the bookend screen comes from a JSON file that's specified in the &lt;amp-story-bookend&gt; tag. For our tutorial, we already have a JSON file (bookend.json) that contains the bookend data.", "If you refresh your browser and go to the last screen, you'll see the following bookend:", "Every bookend screen requires a bookendVersion, which is v1.0 for this tutorial:", "Social share buttons allow readers to share your content through social platforms, like Twitter, Facebook, Pinterest, and so on. You specify social share providers in a shareProviders object, and create an array containing type names for each of the social platforms.", "For this tutorial, we chose Facebook, Twitter, and email for our share providers:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@id.md", ["heading", "small", "landscape", "portrait", "cta-link", "Type", "Description", "There's more to learn about the bookend component. For details, see the amp-story reference documentation.", "The information on the bookend screen comes from a JSON file that's specified in the &lt;amp-story-bookend&gt; tag. For our tutorial, we already have a JSON file (bookend.json) that contains the bookend data.", "Every bookend screen requires a bookendVersion, which is v1.0 for this tutorial:"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@it.md", ["heading", "small", "landscape", "portrait", "cta-link"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@ja.md", ["heading", "small", "landscape", "portrait", "cta-link", "Type", "Description"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@ko.md", ["heading", "small", "landscape", "portrait", "cta-link", "Type", "Description"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@pl.md", ["heading", "small", "landscape", "portrait", "cta-link"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@pt_BR.md", ["heading", "small", "landscape", "portrait", "cta-link"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@tr.md", ["heading", "small", "landscape", "portrait", "cta-link"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@vi.md", ["heading", "small", "landscape", "portrait", "cta-link", "Type"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_bookend@zh_CN.md", ["heading", "small", "landscape", "portrait", "cta-link", "Type", "Description"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/create_cover_page@de.md", ["Template: Fill", "Template: Vertical", "Template: Horizontal", "Template: Thirds"]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/index@fr.md", ["In this tutorial, we'll introduce you to the amp-story component, which you can use to create visually engaging Web Stories with AMP. By the end of this tutorial, you'll have created a story about \"The Joy of Pets\" that provides bite-sized information and visuals to entertain and engage readers."]], 

["pages/content/amp-dev/documentation/guides-and-tutorials/start/visual_story/setting_up@fr.md", ["After setting up your local web server, have a look at what our completed Web Story will look like by the end of this tutorial by accessing the following URL:", "Apache", "nginx"]], 

["pages/content/pixi/no-field-data@id.md", ["Unfortunately, we do not have sufficient real-world performance data for this page.  You could use another URL that uses the same template and has sufficient traffic to get field results. Alternatively, you can look at the lab data or use the Search Console Performance report.  Our data is based on the Chrome User Experience Report which aggregates real-world speed data from opted-in users and requires that a URL must be public (crawlable and indexable) and have sufficient number of distinct samples that provide a representative, anonymized view of performance of the URL."]]]