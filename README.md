# flutterpayphone

Plugin de Flutter para pasarela de pagos Payphone.

Plugin creado por Irwin Ortiz <irwing844@gmail.com>
https://github.com/irwing844/flutter_payphone

## Uso

1. Obtener el Token para el RUC en https://appdeveloper.payphonetodoesposible.com/
2. Llamar a Payphone(tokenApiKey).saleRequest(phoneNumber,amount,amountWithTax,tax,clientTransactionId);
    Esto nos json con un numero de transacción si es que todo salió bien o un codigo de error.
3. Llamar a Payphone(tokenApiKey).saleStatus(clientTransactionId); para verificar si la transaccion es aprobada.

Nota: el clientTransactionId es una referencia cualquiera para identificar la transacción del cliente. 

## Apoyame
Si te sirve este plugin y quieres que sea actualizado constantemente puedes apoyarme donando a mi PayPal: https://www.paypal.me/irwinortiz