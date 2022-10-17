**Disclaimer:** This plugin is provided with no support or guarantees. Testing/development is done for this, but I'd still recommend doing a quick test on a development site before loading on production, to be sure there aren't any issues with a specific site. If you have an issue or suggestion, please submit an issue or PR in the repository on GitHub. Thanks for being part of the WordPress community!

# Pause Renewal Actions
This mini-plugin allows a WooCommerce store to pause all WooCommerce Subscription renewals.

### Notes
- This stops actions with the `woocommerce_scheduled_subscription_payment` hook from being claimed by action scheduler, effectively pausing them.
- As soon as they are unpaused, any past-due actions will start to run.
- This does not pause any other actions, such as failed payment retries.
- This doesn't affect the old PayPal Standard subscriptions; it only works with subscriptions managed from within WC ( Most are ).

### Changelog
2022-10-17 - Version 1.0.0