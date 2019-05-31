# k8-deploy-helper
Helper script for kubectl deployments using minimal requirements. (bash, grep, sed, base64)
Offers:
 - Easy substitution             -- {{MY_VARNAME}}
 - Reading from user input       -- {{MY_VARNAME | READ}}
 - Reading from file             -- {{MY_VARNAME | FILE:<filepath>}}
 - Base64 encoding for secrets   -- {{MY_VARNAME | BASE64}}

Options are combineable, e.g.: {{MY_VARNAME | READ | BASE64}}
Note:
  Plain text multiline file inputs are not supported yet (due to indentation)
  When using base64 encoding this is fine
