# Tutorial de Compute

_Visita el video-tutorial en_ [_YouTube_](https://youtu.be/YFgXMpQszpM)_._

![](https://lh6.googleusercontent.com/JT1YyvA-AYlAGqlIVd-7Vg2NhPuO8rU_hoNX8z1XigAf1PN2ieWIuaBeY_PubKm8kGtMFy09qN_I-pOdtYjK2C9Ab3PO9HvOx3eG_E7y9PCq-WZf7zjWNdy_2eHf4kH2R6A2kPCm)

\(0:24\) Comienza en tu página principal de la consola AWS. Puedes acceder al panel de control de cuenta IAM buscándolo o utilizando el menú desplegable \(0:30\)

![](../.gitbook/assets/image%20%286%29.png)

y clicando en el enlace

![](../.gitbook/assets/image%20%281%29.png)

\(0:36\)

Clica en users, y después en add user. \(0:40\)

![](https://lh3.googleusercontent.com/HHrPPunj5VTQg9tBrVeT0sAzZ48j3M3cRV9sI-jd0W28wiGPVB74CS14nxmxTvWDXS4LF1hc3TX26afnF5yzpjOiWY9BTsqGw-Fy-vCuUmMgwyZXSLHImdepZ_IFujIazDYvVwcl)

Da un nombre a tu nuevo usuario -- el mío será numerai\_train. Bajo el tipo de acceso, selecciona programmatic access, y clica en next. \(0:50\)

![](https://lh6.googleusercontent.com/UQzDp2KWesCZhe9jb0idCiNI7yszgq3fyYWIldPI-EUx-IGqWW1QgwtU6j24usHJz94j7_7z05rjrGGV_urj1kgZfEXBmFfDMMTFKEtc91cZv1rBiuvvj7R0qJn3XJkXeIgfZ-XE)

Ahora selecciona attach existing policies directly, y clica en la primera caja para tener acceso de administrador. Clica next. \(0:58\)

No necesitas añadir etiquetas, así que clica next de nuevo. un clic final crea tu nuevo usuario. El nuevo usuario ha sido creado, y la página muestra tu clave pública y oculta la clave privada. Voy a descargar el CSV de manera que pueda almacenar mis claves de la API numerai. \(1:08\)

![](https://lh3.googleusercontent.com/GoNx8KnC6ytT467kMRPLqVKTHV-qHniUolbz3m1lVR3wh2KFN4redjSk7YJKM2jI4UmE_HSMg6VKLCgE_WD11L0VzSfk3TBI9gBdOf-ga6wbjf45yGJ9LMEIn1ym_7wSYylUEriM)

![](https://lh5.googleusercontent.com/6ihfmBIuTe-4BFEUzqwQeQa0v8sMkhrgepSJxQaBQErtNDjAYpjLgXAW2jfHh48xzxmxeae6n6EVeqvcMSePfwyp5LvlCchJkPRuKZfcviyfZ_ZEhXUQ1yAayvQn40UNux_ZcG6h)

A continuación, abre tu página de settings en la cuenta de numerai y selecciona Add. \(1:31\)

![](https://lh5.googleusercontent.com/zqGTjBjlR_RvBXQlZXhYjVg1bWCHo7BGpqvhjzpZwtbgW2atUE-fIdGK7cP8xe7J2b8n48VOTQ9QSGWB3FBUIdxa7XhWLXcFWAxgFqlHMj2Ub-HFbL7AJPwRj35a78QtGCYvheKN)

Pon nombre a tu clave, y selecciona “upload submissions”, “make stakes”, “view historical submission info” y “view user info”. Escribe tu contraseña y clica generate key. \(1:48\) 

![](https://lh3.googleusercontent.com/ociyl3axYtpsX4Om_2RkV3WjG5xL4UsB-zm7TcGu6S8Y8Ke-ZgFntY-CASfvm5QQ6XBjlsGx_CSYxplgDh7oe_uHJROz2UahQQZLtL7_0U1yhONIvSC84kYre3boOB7v-kwjrRSf)

Copia la clave secreta que se muestra en la caja emergente en la esquina izquierda inferior. \(1:53\)

![](https://lh5.googleusercontent.com/mB9G0owNROjyM0dAU08YCG7qRyJSKVqTpI6HyDpWd4KMB5XG5Dm_v3MMy_mYI0aGVCIQznqYkSYv_3dK2YvRuWcueAy1MVoC80O_2pvCKyooL7KPNCYQVl8_B5N4dGpJlwwsfYcf)

Puedes gurdar esta clave en el CSV que descargaste de AWS. Recopila también la clave pública \(2:04\)

_**Nota: El acceso y las claves secretas proporcionan control sobre tus cuentas AWS y Numerai. Mantenlas seguras como tus nombres de usuario y contraseñas!**_

![](https://lh3.googleusercontent.com/epoIhcwStnpCFXueAGOhZwKmM9-TqLJXCrtLY4cBAUaKSF5wWeh8y32MJGuEyMGUMfft0j5j43oeUHKK9dwUCCFDRa44I4k8Gd5igP49ewR-NEtLQ0DU3aQLGIfUz7k1UUIBMi_J)

Guarda la clave pública en el CSV. A continuación, abre tu anaconda e instala numerai\_cli con pip3. \(2:23\) 

![](https://lh6.googleusercontent.com/zZHb0hph83WJ4ypaUBhmpDu1wHoNXCJKeuVmWswTrweUd2mFJc8zARD8Osis5RcJA3conQOS0kbLSUM-wmCB9hqDoif-lnjDtiwtFQCjrk1mm6QZgBeBtQgv9Y6Fig9l_x0hTP4H)

una vez instalado, escribe mkdir example-numerai, luego cd example-numerai, y numerai setup. \(2:42\) 

![](https://lh4.googleusercontent.com/7_w6V8l6sqcqjPc_XNf1pq3HJmEZwVmg68w4XqoM5i2hrmQXNG2gNXkxDg7aP-Q0vZia_jsaMg8Leg9TddHbq3V56JszLoz3ydGvtsGpuh5CZ92dEK8orM8xNh0efP4_kTt-crnX)

Ahora, copia y pega las claves como se pide la ventana de comandos. \(3:15\)

![](https://lh4.googleusercontent.com/C0zbxWABUMpQwAsPtMb78XvyfnRa6c4bZT1F4hyvJkA8aFuBuR_hSQv7Pn_xZVMj52grXKaAVxvYeHhPE__NfNk-G7HynDlGuReAqoLDia-lqpSUxNgGC8yXV5YvCU1M8SudPyKS)

Deberías ver un conjunto de mensajes mostrando que has instalado numerai-cli correctamente. \(3:41\)

![](https://lh5.googleusercontent.com/L3DVgnjU_cxeU2Sv7WP-u6gYrPjlgCYuD9hzHlqovS9RdqjeOLISoZ_SyWwFFTj8DIfEcEaeb56CJjas0HE2VgUyZFUpa5kp-Olos6ssUdAxkp923NvITZWo4a6tFH0HsVFklkWK)

Escribe numerai docker copy-example. Esto nos da todos los nombres de fichero y código de ejemplo que podemos sobreescribir. \(3:56\)

![](https://lh6.googleusercontent.com/4Z-cFieomwv8gV2d9BtBdltBGsU3Eel9QhYSk01E5h2kIFam5cebN-xAFHIxWw8yjxB6JEnMI45SLbgyPJtyNaxlwyVoCeS6riADOhNm8-Ab399ysh4syyjuvLPKxf-jOnOkUs-v)

Ahora voy a ejecutar un modelo muy sencillo de regresión utilizando RidgeCV de scikit-learn. Guardaremos este modelo usando joblib. Escribe numerai docker train. Docker ejecuta el fichero trin.py, que descarga los datos, ajusta el modelo, y guarda el modelo usando joblib. Te ahorraré el aburrimiento de ver los datos descargarse y la espera a que el modelo se entrene. Como puedes ver, el fichero joblib se ha guardado en el directorio example\_numerai junto con el dataset de numerai. \(4:28\)

![](https://lh6.googleusercontent.com/MQayrwIgIVnj-D0JjNUuFDRl1De9GBxvOpwRn5tsz7lr6F7dYlnBgbG5H_xA9U9ZF0HY2AFJyS2YPaEsrLJ5pq7VWVTSkbyrJzSZIh-A5rzYrU3X2-rZ2N61sz4vhg9ebaWeOUt7)

Queremos asegurarnos de que el modelo funciona correctamente antes de llevar nuestra imagen del docker a AWS. Escribe numerai docker run. Esto creará la imagen del docker y ejecutará predict.py en tu máquina. Una vez que tu modelo termine de generar las predicciones, numerox enviará tus predicciones usando las claves API que proporcionaste. \(4:51\)

![](https://lh3.googleusercontent.com/OkYPLYPpsNtp-r15IlxfQOdrpSWuqFVJqwTRZQ8sJ8ZdZkFIiMGSiz6pl3iLIkfDcW4YTVh5QAo8UVnrHrN0FQ6RaXnYUH8mlrGLHFHwx4xbixxw6NyzvCn13xC5hLiaTMRwIbuT)

Cojamos la dirección webhook. Navega a .numerai en el directorio example\_predictions. \(4:59\)

![](https://lh3.googleusercontent.com/-qIvZJdaYN-MixvSEDTxFesieZK_cEq8exyzoi8Vh2HH3Ff9TM_wY7qTQ_PFRxeN9PD4kboBFSFr837S1Uwj55hFzCLUnkjmkAGU5CUVBZ_UFzxeTRxDsTtdaLdgtdkLFL_yyskP)

Abre submission\_url.txt y copia la dirección. \(5:03\)

![](https://lh6.googleusercontent.com/-tDzCP5PvZuNDr2KLUswWdNm-SQGsIYFypCaqpkMLMjrV-HYGKal3jH5a75AZ7zBrBKYg5ih7MWCyOdpDWNfJlDpykxyO1pchg8RWUHOJTStos4-MSLRwjyuqim9yVyu29ogk4qC)

Abre la página de settings de tu cuenta de Numerai de nuevo, clica Compute, pega la dirección en el campo, y clica change webhooks. \(5:15\)

![](https://lh3.googleusercontent.com/FIJeEii3ArKQwjrhzkLKniCKSo_KIIYbrB0TFgOad6C6mGhyyY6XJ05jf45sqQ9_w1gqY1BCERnj6LCPx-KKscZDGdMXwpmtyhGCVavoYZzCN3QKs9wyKWgvhz47dyzbxNG_pZNu)

Como puedes ver, el último envio muestra que nuestro test local fue un éxito. \(5:23\)

![](https://lh4.googleusercontent.com/Kj7BZsN4ZiJ-3-FUaW9b17PZmAJam6xUJTxKjXzdx9Z3HReUKtdKUr6cghw7i9eV0h1XcEPjV4p5bOwPK6Ao6f-pyltBPs5IEjL0onYprWPyUuSL1NYVhYvcp9SuNAUN6TR6wnYS)

Escribe **numerai docker deploy** y espera a que tus ficheros docker se envíen a AWS. \(5:48\)

![](https://lh3.googleusercontent.com/BknJF6TzVUKr01EnAUA_eeAZQTjxI3UDhaBhyfA_i09DFcRHZrWwWRcjiUzkCXsdK3QuHHk-Qmq9poDBdVvZetql2wo4ecQYSqMH4c-TW-HOq4IOz4mOfscYjsfsvK0pu3jifWqB)

Comprueba el webhook escribiendo numerai compute test-webhook. Puedes obtener tus logs escribiendo numerai compute logs -f.   
Cuando veas el mensaje “Task is now in the DEPROVISIONING state", tu código ha terminado. \(6:37\)

![](https://lh6.googleusercontent.com/UMDqrC30nc0b8EhpEKK5WilfPFAIj1Jy2T-CJo2PTqtfnzL-inv5TYe6MvQ7lrdCqcvuPH910wRvsmQGl-ZVDHQJd6zPZoWfKLz1wTLY-vEIbyybeCGGg6bWhMGhutEplTwvt-Z8)

_Enhorabuena, ahora eres libre para disfrutar de tus sábados!_



