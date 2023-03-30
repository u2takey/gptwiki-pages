# stripe 
## chatgpt 
Stripe is not a command, but rather a payment processing service for businesses. It allows businesses to accept payments online, both on their website or mobile app, as well as in-store. Stripe provides a simple and secure way for businesses to process payments and manage their revenue. To use Stripe, businesses can sign up for an account on the Stripe website, and then integrate Stripe's payment processing functionality into their own website or app. Stripe offers a range of features, such as support for multiple payment methods and currencies, recurring payments, and fraud protection. Businesses can also manage their payments and customer data through the Stripe dashboard, which provides insights into revenue, transaction history, and customer behavior. Overall, Stripe provides a powerful and flexible payment processing solution for businesses of all sizes. 

## tldr 
 
> Interact with a Stripe account.
> More information: <https://github.com/stripe/stripe-cli>.

- Follow the logs of activity on the account:

`stripe logs tail`

- Listen for events, filtering on events with the name `charge.succeeded` and forwarding them to localhost:3000/events:

`stripe listen --events="{{charge.succeeded}}" --forward-to="{{localhost:3000/events}}"`

- Send a test webhook event:

`stripe trigger {{charge.succeeded}}`

- Create a customer:

`stripe customers create --email="{{test@example.com}}" --name="{{Jenny Rosen}}"`

- Print to JSON:

`stripe listen --print-json`
