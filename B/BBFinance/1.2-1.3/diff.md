# Comparing `tmp/BBFinance-1.2.tar.gz` & `tmp/BBFinance-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.2.tar", last modified: Fri Apr  7 23:16:48 2023, max compression
+gzip compressed data, was "BBFinance-1.3.tar", last modified: Fri Apr  7 23:25:57 2023, max compression
```

## Comparing `BBFinance-1.2.tar` & `BBFinance-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 23:16:48.317080 BBFinance-1.2/
-drwxrwxrwx   0        0        0        0 2023-04-07 23:16:48.291104 BBFinance-1.2/BBFinance/
--rw-rw-rw-   0        0        0    25436 2023-04-07 23:15:29.000000 BBFinance-1.2/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      289 2023-04-07 23:16:39.000000 BBFinance-1.2/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 23:16:48.315084 BBFinance-1.2/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     1995 2023-04-07 23:16:48.000000 BBFinance-1.2/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-07 23:16:48.000000 BBFinance-1.2/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 23:16:48.000000 BBFinance-1.2/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      255 2023-04-07 23:16:48.000000 BBFinance-1.2/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-07 23:16:48.000000 BBFinance-1.2/BBFinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1099 2023-04-07 01:44:35.000000 BBFinance-1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1995 2023-04-07 23:16:48.316075 BBFinance-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-04-07 01:44:35.000000 BBFinance-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-07 23:16:48.317080 BBFinance-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1294 2023-04-07 23:13:24.000000 BBFinance-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:25:57.736825 BBFinance-1.3/
+drwxrwxrwx   0        0        0        0 2023-04-07 23:25:57.720824 BBFinance-1.3/BBFinance/
+-rw-rw-rw-   0        0        0    25646 2023-04-07 23:25:52.000000 BBFinance-1.3/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      289 2023-04-07 23:16:39.000000 BBFinance-1.3/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:25:57.734825 BBFinance-1.3/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     1995 2023-04-07 23:25:57.000000 BBFinance-1.3/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-07 23:25:57.000000 BBFinance-1.3/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 23:25:57.000000 BBFinance-1.3/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      255 2023-04-07 23:25:57.000000 BBFinance-1.3/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-07 23:25:57.000000 BBFinance-1.3/BBFinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1099 2023-04-07 01:44:35.000000 BBFinance-1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1995 2023-04-07 23:25:57.736825 BBFinance-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-04-07 01:44:35.000000 BBFinance-1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-07 23:25:57.737824 BBFinance-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2023-04-07 23:22:11.000000 BBFinance-1.3/setup.py
```

### Comparing `BBFinance-1.2/BBFinance/BBFinance.py` & `BBFinance-1.3/BBFinance/BBFinance.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     df[nomeColuna] = df[nomeColuna].replace('[%]', '', regex=True)
     df[nomeColuna] = df[nomeColuna].replace('[,]', '.', regex=True)
     df[nomeColuna] = df[nomeColuna].astype(float)
 
     return df
 
 ## INFOS DAS AÇOES ##
-@app.get("/stocks/{symbol}/info")
+@app.get("/stocks/{symbol}/info", response_model=None)
 def get_info(symbol: str) -> dict:
     
     """
     ## Usabilidade 
     - Busca as principais informaçoes sobre o ativo selecionado como Preço e Dividendos \n
     
     ## Parâmetros
@@ -96,15 +96,15 @@
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/info")
 response = Response(media_type="application/json")
 
 
 ## HISTORICO DAS AÇOES ##
 
-@app.get("/stocks/{symbol}/history")
+@app.get("/stocks/{symbol}/history", response_model=None)
 def get_stock_history(symbol: str, period: str = '1y') -> pd.DataFrame:
     
     """
     ## Usabilidade 
     - Usada para verificar o histórico da açao selecionada e em qual periodo \n
     
     ## Parâmetros
@@ -141,15 +141,15 @@
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/history")
 responseHistory = Response(media_type="application/json")
 
 
 ## TENDENCIA DE PREÇO ##
 
-@app.get("/stock/{symbol}/trend")
+@app.get("/stock/{symbol}/trend", response_model=None)
 def get_stock_trend(symbol: str) -> dict:
     
     """
     ## Usabilidade 
     - Identifica a tendencia de preço de uma açao, se ira ser de ALTA ou BAIXA
     
     ## Parâmetros
@@ -181,15 +181,15 @@
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/trend")
 responseHistory = Response(media_type="application/json")
 
 
 ## RSI ##
 
-@app.get("/stock/{symbol}/technical")
+@app.get("/stock/{symbol}/technical", response_model=None)
 def get_stock_technicals(symbol: str) -> dict:
     
     """
     ## Usabilidade 
     - cálculo envolve a comparação da média de ganhos em um período de tempo com a média de perdas em um período de tempo. \n
     
     ## Como interpretar 
@@ -245,15 +245,15 @@
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/technical")
 responseHistory = Response(media_type="application/json")
 
 
 ## VOLATILIDADE ##
 
-@app.get("stocks/{symbol}/volatility")
+@app.get("stocks/{symbol}/volatility", response_model=None)
 def get_volatility(symbol: str, start_date: str, end_date: str) -> str:
     
     """
     ## Usabilidade 
     - Método usado para verificar a volatilidade de um ativo em comparacao ao mercado em que esta  \n
     
     ## Parâmetros
@@ -276,15 +276,15 @@
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/volatility")
 responseHistory = Response(media_type="application/json")
 
 
 ## BETA ##
 
-@app.get("stocks/{symbol}/beta")
+@app.get("stocks/{symbol}/beta", response_model=None)
 def get_beta(symbol: str) -> dict:
     
     """
     ## Usabilidade 
     - O beta é uma medida estatística que indica a relação entre a volatilidade de uma ação e a volatilidade do mercado como um todo.
     O valor do beta é utilizado para medir o risco de uma ação em relação ao mercado em que ela é negociada. \n
     
@@ -334,15 +334,15 @@
 if __name__ == '__main__':
     uvicorn.run("main:app", host='127.0.0.1', port=8000, default="stocks/{symbol}/beta")
 responseHistory = Response(media_type="application/json")
 
 
 ## VAR ##
     
-@app.get("stocks/{symbol}/VaR")
+@app.get("stocks/{symbol}/VaR", response_model=None)
 def get_var(symbol: str, confidence_level: float, lookback_period: int) -> dict:
     
     """
     ## Usabilidade 
     - O Value at Risk (VaR) é uma medida de risco que indica a perda máxima esperada, com um determinado nível de confiança, em um intervalo de tempo pré-determinado. \n
     
     ## Parâmetros
@@ -483,15 +483,15 @@
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="stocks/{symbol}/AnnualReturn")
 responseHistory = Response(media_type="application/json")
 
 
 ## ALOCAÇAO DE MARKOWITZ ##
 
-@app.get("stocks/{symbol}/MarkowitzAllocationn")
+@app.get("stocks/{symbol}/MarkowitzAllocationn", response_model=None)
 def markowitz_allocation(symbols= list, star_date= str, end_date=str) -> str: 
     
     """
     ## Usabilidades 
     Alocação de Markowitz é uma técnica de otimização de portfólio que visa encontrar a combinação ideal de ativos para maximizar o retorno do investimento enquanto minimiza o risco. \n
     
     ## O Retorno Esperado
@@ -569,15 +569,15 @@
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="/infoFunds")
 responseHistory = Response(media_type="application/json")
 
 
 ## COMPARADOR DE FUNDOS COM BASE NO SETOR ##
 
-@app.get("/compareSetorFunds")
+@app.get("/compareSetorFunds", response_model=None)
 def compare_setor_funds(setor= TipoSetores, rentabilidade_min = 0) -> pd.DataFrame:
     
     """
     ## Usabilidade
     
     - Funçao que utiliza as metricas e medias dos fundo com base no seu Setor para uma analise mais restrita
     
@@ -638,15 +638,15 @@
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=8000, default="/compareSetorFunds")
 responseHistory = Response(media_type="application/json")
 
 
 ## COMPARADOR DE FUNDOS ##
 
-@app.get("/compareFunds")
+@app.get("/compareFunds", response_model=None)
 def compare_funds(listfund= None, fund_1= str, fund_2= str) -> pd.DataFrame:
     """
     ## Usabilidade 
     
     - Funçao que realiza a comparaçao entre dois fundos, seja feita a requisiçao dos fundos via lista ou unicos 
     - Requisiçao Listas: Retorna o fundo com maior porcentagem de risco (a variação percentual dos preços dos ativos, calculo realizado com base no desvio padrão)
     - Requisiçao Unica: Retorna um Dataframe com as principais informaçoes dos fundos, afim de uma comparaçao entre seus valores \n
```

### Comparing `BBFinance-1.2/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.3/BBFinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.2
+Version: 1.3
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.2/LICENSE.txt` & `BBFinance-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.2/PKG-INFO` & `BBFinance-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.2
+Version: 1.3
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.2/README.md` & `BBFinance-1.3/README.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.2/setup.py` & `BBFinance-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.2',
+    version='1.3',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='MIT',
     packages=['BBFinance'],
     long_description= long_description,
```

