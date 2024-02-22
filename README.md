

<p align="center"> <img src="https://user-images.githubusercontent.com/50652676/62349836-882fef80-b51e-11e9-99e3-7b974309c7e3.png" width="100" height="100"></p>


<h1 align="center">
    Terraform AWS labels
</h1>

<p align="center" style="font-size: 1.2rem;">
    Terraform module to create labels resource on AWS.
     </p>

<p align="center">

<a href="https://www.terraform.io">
  <img src="https://img.shields.io/badge/Terraform-v1.1.7-green" alt="Terraform">
</a>
<a href="LICENSE.md">
  <img src="https://img.shields.io/badge/License-APACHE-blue.svg" alt="Licence">
</a>






## Prerequisites

This module has a few dependencies:

- [Terraform 1.x.x](https://learn.hashicorp.com/terraform/getting-started/install.html)
- [Go](https://golang.org/doc/install)







## Examples


**IMPORTANT:** Since the `master` branch used in `source` varies based on new modifications, we suggest that you use the release versions [here](https://github.com/slovink/terraform-aws-labels/releases).


### Simple Example
Here is an example of how you can use this module in your inventory structure:
  ```hcl
 module "labels" {
  source = "./../"

  name        = "labels"
  environment = "test"
  label_order = ["name", "environment"]
  attributes  = ["private"]
}
  ```
## License
This Terraform module is available under the MIT License. For more details, please see the [LICENSE](https://github.com/slovink/terraform-aws-labels/blob/vinod/LICENSE) file.


## Feedback
If you come accross a bug or have any feedback, please log it in our [issue tracker](https://github.com/slovink/terraform-aws-labels/issues), or feel free to drop us an email at [devops@slovink.com](mailto:devops@slovink.com).

If you have found it worth your time, go ahead and give us a ★ on [our GitHub](https://github.com/slovink/terraform-aws-labels)!
