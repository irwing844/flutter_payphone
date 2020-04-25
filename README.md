# flutterpayphone

Plugin de Flutter para pasarela de pagos Payphone.

Plugin creado por Irwin Ortiz <irwing844@gmail.com>

## Uso

1. Obtener el Token para el RUC en https://appdeveloper.payphonetodoesposible.com/
2. Llamar a Payphone(tokenApiKey).saleRequest(phoneNumber,amount,amountWithTax,tax,clientTransactionId);
    Esto nos devuelve un json con un número de transacción si es que todo salió bien, o un codigo de error.
3. Llamar a Payphone(tokenApiKey).saleStatus(clientTransactionId); para verificar el status de la transacción.

Nota 1: el clientTransactionId es una referencia cualquiera para identificar la transacción del cliente. 

Nota 2: Amount, AmountWithTax y Tax . 

## Apoyame
Si te sirve este plugin y quieres que sea actualizado constantemente puedes apoyarme donando a mi PayPal: https://www.paypal.me/irwinortiz