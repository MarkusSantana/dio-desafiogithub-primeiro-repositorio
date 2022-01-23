```python
!pip install requests

```

    Collecting requests

    WARNING: You are using pip version 21.2.3; however, version 21.3.1 is available.
    You should consider upgrading via the 'C:\Users\mvcsa\AppData\Local\Programs\Python\Python310\python.exe -m pip install --upgrade pip' command.
    

    
      Downloading requests-2.26.0-py2.py3-none-any.whl (62 kB)
    Collecting charset-normalizer~=2.0.0
      Downloading charset_normalizer-2.0.7-py3-none-any.whl (38 kB)
    Collecting certifi>=2017.4.17
      Downloading certifi-2021.10.8-py2.py3-none-any.whl (149 kB)
    Collecting urllib3<1.27,>=1.21.1
      Downloading urllib3-1.26.7-py2.py3-none-any.whl (138 kB)
    Collecting idna<4,>=2.5
      Downloading idna-3.3-py3-none-any.whl (61 kB)
    Installing collected packages: urllib3, idna, charset-normalizer, certifi, requests
    Successfully installed certifi-2021.10.8 charset-normalizer-2.0.7 idna-3.3 requests-2.26.0 urllib3-1.26.7
    


```python
import requests
```


```python
url = 'https://api.exchangerate-api.com/v6/latest'

req = requests.get(url)

print(req.status_code)
```

    200
    


```python
dados = req.json()

print(dados)
```

    {'result': 'success', 'provider': 'https://www.exchangerate-api.com', 'documentation': 'https://www.exchangerate-api.com/docs/free', 'terms_of_use': 'https://www.exchangerate-api.com/terms', 'time_last_update_unix': 1637712151, 'time_last_update_utc': 'Wed, 24 Nov 2021 00:02:31 +0000', 'time_next_update_unix': 1637799261, 'time_next_update_utc': 'Thu, 25 Nov 2021 00:14:21 +0000', 'time_eol_unix': 0, 'base_code': 'USD', 'rates': {'USD': 1, 'AED': 3.67, 'AFN': 94.12, 'ALL': 108.82, 'AMD': 481, 'ANG': 1.79, 'AOA': 595.04, 'ARS': 100.83, 'AUD': 1.38, 'AWG': 1.79, 'AZN': 1.72, 'BAM': 1.73, 'BBD': 2, 'BDT': 86.63, 'BGN': 1.73, 'BHD': 0.376, 'BIF': 2002.29, 'BMD': 1, 'BND': 1.36, 'BOB': 6.93, 'BRL': 5.61, 'BSD': 1, 'BTN': 74.77, 'BWP': 11.73, 'BYN': 2.51, 'BZD': 2, 'CAD': 1.27, 'CDF': 2035.28, 'CHF': 0.932, 'CLP': 810.81, 'CNY': 6.39, 'COP': 3910.96, 'CRC': 642.94, 'CUC': 1, 'CUP': 25, 'CVE': 97.53, 'CZK': 22.67, 'DJF': 177.72, 'DKK': 6.6, 'DOP': 56.93, 'DZD': 140.39, 'EGP': 15.8, 'ERN': 15, 'ETB': 48.93, 'EUR': 0.885, 'FJD': 2.11, 'FKP': 0.747, 'FOK': 6.6, 'GBP': 0.747, 'GEL': 3.16, 'GGP': 0.747, 'GHS': 6.18, 'GIP': 0.747, 'GMD': 53.49, 'GNF': 9718.34, 'GTQ': 7.77, 'GYD': 212.84, 'HKD': 7.79, 'HNL': 24.38, 'HRK': 6.66, 'HTG': 99.78, 'HUF': 330.24, 'IDR': 14181.21, 'ILS': 3.13, 'IMP': 0.747, 'INR': 74.78, 'IQD': 1483.74, 'IRR': 42371.97, 'ISK': 131.29, 'JMD': 156.63, 'JOD': 0.709, 'JPY': 114.93, 'KES': 112.85, 'KGS': 85.52, 'KHR': 4138.94, 'KID': 1.38, 'KMF': 435.14, 'KRW': 1190.69, 'KWD': 0.3, 'KYD': 0.833, 'KZT': 435.01, 'LAK': 10838.36, 'LBP': 1507.5, 'LKR': 203.27, 'LRD': 144.74, 'LSL': 15.83, 'LYD': 4.67, 'MAD': 9.26, 'MDL': 17.81, 'MGA': 4017.57, 'MKD': 55.03, 'MMK': 1789.22, 'MNT': 2898.69, 'MOP': 8.03, 'MRU': 36.87, 'MUR': 43.67, 'MVR': 15.55, 'MWK': 822.25, 'MXN': 21.15, 'MYR': 4.2, 'MZN': 64.61, 'NAD': 15.83, 'NGN': 424.12, 'NIO': 35.63, 'NOK': 8.93, 'NPR': 119.63, 'NZD': 1.44, 'OMR': 0.384, 'PAB': 1, 'PEN': 4.03, 'PGK': 3.56, 'PHP': 50.73, 'PKR': 176.16, 'PLN': 4.19, 'PYG': 6858.07, 'QAR': 3.64, 'RON': 4.4, 'RSD': 105.21, 'RUB': 74.96, 'RWF': 1035.36, 'SAR': 3.75, 'SBD': 8.07, 'SCR': 13.18, 'SDG': 445.6, 'SEK': 9.01, 'SGD': 1.36, 'SHP': 0.747, 'SLL': 11139.91, 'SOS': 588.37, 'SRD': 21.9, 'SSP': 312.13, 'STN': 21.67, 'SYP': 2553.19, 'SZL': 15.83, 'THB': 33.1, 'TJS': 11.38, 'TMT': 3.53, 'TND': 2.88, 'TOP': 2.27, 'TRY': 12.37, 'TTD': 6.83, 'TVD': 1.38, 'TWD': 27.89, 'TZS': 2315.29, 'UAH': 26.83, 'UGX': 3577.95, 'UYU': 44.39, 'UZS': 10893.9, 'VES': 4.56, 'VND': 22902.37, 'VUV': 112.63, 'WST': 2.59, 'XAF': 580.19, 'XCD': 2.7, 'XDR': 0.716, 'XOF': 580.19, 'XPF': 105.55, 'YER': 252.71, 'ZAR': 15.83, 'ZMW': 17.76}}
    


```python
valor_reais = float(input('Informe o valor a ser convertido em R$:\n'))
cotacao = dados['rates']['BRL']
print(f'R${valor_reais} em dólar valem US$ {(valor_reais / cotacao):.2f}')
```

    Informe o valor a ser convertido em R$:
    500
    R$500.0 em dólar valem US$ 89.13
    


```python

```
