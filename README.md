# flutter_payphone

Plugin de Flutter para pasarela de pagos Payphone.

Plugin creado por Irwin Ortiz <irwing844@gmail.com>

## Uso

1. Obtener el Token para el RUC en https://appdeveloper.payphonetodoesposible.com/
2. Puedes llamar a los siguientes métodos:
    * Payphone(tokenApiKey).enviarVentaResultadoWidget(context, widget, phoneNumber,amount,amountWithTax,tax,clientTransactionId, referencia); (Esto nos devuelve un dialog con un widget hasta esperar que el cliente aprueba la transaccion en la APP de Payphone)
    * Payphone(tokenApiKey).enviarVentaResultado(phoneNumber,amount,amountWithTax,tax,clientTransactionId, referencia); (Esto es sin widget)
    * Payphone(tokenApiKey).consultarVenta(clientTransactionId); 
    *enviarAnulacionResultadoWidget, enviarAnulacionResultado y consultarAnulacion (lo mismo que la venta)   
    (Esto nos devuelve un json con un número de transacción si es que todo salió bien, o un codigo de error)

Nota 1: El clientTransactionId es una referencia cualquiera para identificar la transacción del cliente (debe ser único). 
Nota 2: Amount, AmountWithTax y Tax se deben multiplicar por 100, es decir, $1 dólar = 100; $1.50 dólares = 150.
Nota 3: La referencia es el concepto del cobro. 

## Apoyame
Si te sirve este plugin y quieres que sea actualizado constantemente puedes apoyarme donando 
a mi cuenta de payphone:
 
 ![https://ppls.me/Tge8Brvr2u8yjBLHKI5A](https://raw.githubusercontent.com/irwing844/flutter_payphone/master/link_pago_flutter.jpeg)


O lo puedes hacer a mi PayPal: https://www.paypal.me/irwinortiz