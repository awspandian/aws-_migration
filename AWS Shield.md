• AWS Shield is a managed Distributed Denial of Service (DDoS) protection service
• Safeguards web application running on AWS with always-on detection and automatic inline mitigations
• Helps to minimize application downtime and latency
• Two tiers –
• Standard – no cost
• Advanced - $3k USD per month and 1 year commitment
• Integrated with Amazon CloudFront (standard included by default)

AWS WAF
• AWS WAF is a web application firewall
• WAF lets you create rules to filter web traffic based on conditions that include IP addresses, HTTP headers and body, or custom URIs
• WAF makes it easy to create rules that block common web exploits like SQL injection and cross site scripting
• Web ACLs – You use a web access control list (ACL) to protect a setof AWS resources
• Rules – Each rule contains a statement that defines the inspection criteria, and an action to take if a web request meets the criteria
• Rule groups – You can use rules individually or in reusable rule groups
• IP Sets - An IP set provides a collection of IP addresses and IP address ranges that you want to use together in a rule statement
• Regex pattern set - A regex pattern set provides a collection of regular expressions that you want to use together in a rule statement A rule action tells AWS WAF what to do with a web request when it matches the criteria defined in the rule:
• Count – AWS WAF counts the request but doesn't determine whether to allow it or block it. With this action, AWS WAF continues processing the remaining rules in the web ACL
• Allow – AWS WAF allows the request to be forwarded to the AWS resource for processing and response
• Block – AWS WAF blocks the request and the AWS resource responds with an HTTP 403 (Forbidden) status code
