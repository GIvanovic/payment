# payment
## Ŀ��
��֧������΢��JS����Ǯ�ȵ�����֧�����м��ɣ����������֧�����أ�����������ڵ�֧������

## ���

### ����
t_payment_ext_conf�����ڱ���ͻ�����prepay callback��spring bean����
t_payment_account�����ڱ���֧���˻���������Ϣ
t_payment_transaction�����ڱ���ÿ�ʶ�����ʵ����Ϣ

### ����
1. �����ݿ�����֧���ʺ������Ϣ
2. ������Ʒ������Ϣ��ǩ���󣬲���html��
3. ͨ��http����https���͸�����֧��ƽ̨
4. ҳ����ת������֧��ƽ̨����֧��
5. ֧����ɺ����ǰ̨�ͺ�̨�ص�
6. ǰ̨�ص���Ҫ����չʾ֧�����
7. ��̨�ص���Ҫ���ڽ������

### ������֯��
* payment-common:��һϵ�л����⣬����ǩ�������ڣ���־��

* payment-api: ����һϵ�нӿ�, ����payment-server�����б����á�
** `org.klose.payment.api.PaymentProxy`:������������֧����Ϣ����ѯ֧���˻����õ�
** `org.klose.payment.api.CallBackAgent`: ��̨�ص��е�ҵ���߼�

* payment-runtime: ��PaymentProxy��ӿڵ�ʵ�֡�
** `org.klose.payment.integration`:����Ҫʵ�ָ���֧��ƽ̨�������ݺͺ�̨�����߼�

* payment-server: ҳ��jsp�����restful����
** `testPay.jsp`��������ڣ����ã�org.klose.payment.server.rest.PaymentResource#createPayment�����restful����
** `paymentForm.jsp`������֧������������֧��
** `paymentResult.jsp`��һ����չʾǰ̨�ص���Ĭ��ʵ��


### �ͻ�����

ʵ��'org.klose.payment.server.prepare.PaymentIntegrationService'��׼����Ʒ���۸񣬶����ȸ�����Ϣ
ʵ��'org.klose.payment.api.CallBackAgent'����̨�ص��С����ҵ�����ｻ�ס�


## License
Copyright © 2016 
Distributed under the Appache Public License version 2.0
