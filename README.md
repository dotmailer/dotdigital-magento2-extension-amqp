# Dotdigital AMQP (Magento Open Source and Adobe Commerce)

The Dotdigital AMQP module is an enhancement for the [Dotdigitalgroup Email](https://github.com/dotmailer/dotmailer-magento2-extension) module which enables the integration of [RabbitMQ](https://rabbitmq.com/) or other AMQP brokers as the message queue system. This module overrides the Dotdigitalgroup_Email module queue configurations.

From 2.4.0, queue definitions are supposed to be agnostic, i.e. you state your preference in a runtime configuration. We require a separate module to enable AMQP because we still need to support Magento 2.3.7. In 2.3.7, it is required to specify a connection type (`db`) and
this means our queues don't automatically adapt to `amqp`, even if the deployment configuration specifies this.

## Requirements
- This module requires the Dotdigitalgroup Email module v4.24.0+
- RabbitMQ or other AMQP compatible message broker should be installed and configured.
- PHP 7.4+
- Magento 2.3.7+

## Activation
```
composer require dotdigital/dotdigital-magento2-extension-amqp
bin/magento setup:upgrade
```

## Changelog

### 1.1.0

##### What's new
- We added compatibility with a new queue definition in the Dotdigitalgroup_Email module.

### 1.0.0
- Initial release
