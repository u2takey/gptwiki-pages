# cmctl 
## chatgpt 
Unfortunately, as an AI language model, I do not have information on which specific CMCTL you are referring to. There are multiple CMCTL (or similar acronyms) that can be used within different contexts.

Can you please provide more information or context, so I can understand better what you are looking for? 

## tldr 
 
> A CLI tool that can help you to manage cert-manager resources inside your cluster.
> Check cert signing status, approve/deny requests, and issue new certificate requests.
> More information: <https://cert-manager.io/docs/usage/cmctl/>.

- Check if the cert-manager API is ready:

`cmctl check api`

- Check the status of a certificate:

`cmctl status certificate {{cert_name}}`

- Create a new certificate request based on an existing certificate:

`cmctl create certificaterequest my-cr --from-certificate-file {{cert.yaml}}`

- Create a new certificate request, fetch the signed certificate, and set a maximum wait time:

`cmctl create certificaterequest my-cr --from-certificate-file {{cert.yaml}} --fetch-certificate --timeout {{20m}}`
