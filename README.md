# Dotdigital AMQP (Magento Open Source and Adobe Commerce)

The Dotdigital AMQP module is an enhancement for the [Dotdigitalgroup Email](https://github.com/dotmailer/dotmailer-magento2-extension) module which enables the integration of [RabbitMQ](https://rabbitmq.com/) or other AMQP brokers as the message queue system. This module overrides the Dotdigitalgroup_Email module configurations to provide seamless compatibility with Magento's built-in message queues.

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

