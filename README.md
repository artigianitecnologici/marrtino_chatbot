# marrtino_chatbot
sudo apt install python3.8-venv
sudo apt install python3-pip

python3 -m venv myenv


source myenv/bin/activate
pip3 install -r requirements.txt

source myenv/bin/activate

http://x.x.x.x:5000/query-example?query=ciao


http://127.0.0.1:5000/bot?query=ciao



<category><pattern>MI CHIAMO *</pattern> 
<template>Ciao <set name="nome"><star/></set>, come va?</template>
</category>
<category><pattern>* MI CHIAMO *</pattern> 
<template>Ciao <set name="nome"><star/></set>, come va?</template>
</category>
<category><pattern>* TI CHIAMI</pattern>
<template><srai>PRESENTATI</srai></template>
</category>
<category><pattern>* CHI SEI</pattern>
<template><srai>PRESENTATI</srai></template>
</category>
<category><pattern>PRESENTATI</pattern>
<template>Sono martino il social robot</template>
</category>
<category><pattern>* PRESENTARE</pattern>
<template><srai>presentati</srai></template>
</category>