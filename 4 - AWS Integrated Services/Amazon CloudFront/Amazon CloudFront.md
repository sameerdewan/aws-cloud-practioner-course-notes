# Amazon CloudFront

* Amazon CloudFront uses a global network of over 80 Edge Locations, ever increasing
* You can utilize this to deliver content to your end users with low latency
* The service can be cached to be delivered elsewhere in the world
* Amazon CloudFront is a Content Delivery Network (CDN)
* Integrated closely with:
  * AWS Web Application Firewall
  * AWS Certificate Manager,
  * Amazon Route 53
  * Amazon S3
  * and many others

> Creating a CDN
>
> * Go to the AWS Management Console
>   * Click on Create Distribution
>   * Select CDN type
>     * RTMP is for videos
>     * Web is for normal content delivery, or static
>   * CloudFront can be used to deliver dynamic content too
> * Create Distribution
>   * Select an Origin Domain Name, Path, and ID
>   * You can have multiple origins tied to multiple behaviors
> * Click Create Distribution
> * You can use the AWS CLI to automate CDN creation


> CDN Use Cases
>
> * Static asset caching
> * Live and on demand video streaming
> * Security and DDoS protection
> * Dynamic and customized content
> * API acceleration
> * Software distribution
