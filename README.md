###PHP TUTORIAL: PayPal Instant Payment Notification (IPN)

####描述
Instant Payment Notification (IPN) is a message service that notifies you of events related to PayPal transactions. You can use IPN messages to automate back-office and administrative functions, such as fulfilling orders, tracking customers, and providing status and other transaction-related information.


简单来说，就是在PayPal支付完成后使用IPN的方式获取交易信息。


####使用方法：
1、首先利用如下代码获取PayPal POST过来的数据


    $ipn_post_data = $_POST;


2、调用Paypal_IPN类中的process函数，传入$ipn_post_data，如果验证成功则返回以关联数组组织的交易数据，失败则返回FALSE。


3、更加详细教程请见：http://ethanblog.com/tech/php-for-paypal-instant-payment-notification.html
