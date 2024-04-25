import time
import random
from IPython.display import display, HTML

def coletar_altitude():
    # Simulação de coleta de altitude da aeronave
    altitude = random.randint(0, 40000)  # Simulação de altitude entre 0 e 40000 pés
    return altitude

def gerar_alerta_html(altitude):
    limite_superior = 35000  # Limite superior de altitude permitida
    limite_inferior = 0      # Limite inferior de altitude permitida
    
    if altitude > limite_superior or altitude < limite_inferior:
        alerta_html = '<p style="color:red;">Alerta: Aeronave fora dos limites de altitude! Altitude: {} pés</p>'.format(altitude)
    else:
        alerta_html = '<p>Leitura normal de altitude da aeronave: {} pés</p>'.format(altitude)
    return alerta_html

def simular_coleta(intervalo):
    while True:
        altitude = coletar_altitude()
        alerta_html = gerar_alerta_html(altitude)
        display(HTML(alerta_html))
        time.sleep(intervalo)

# Definindo o intervalo de coleta em segundos
intervalo_coleta = 5

# Iniciando a simulação de coleta de altitude da aeronave
simular_coleta(intervalo_coleta)
