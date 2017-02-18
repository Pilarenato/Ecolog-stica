# Ecolog-stica
import sys

line = sys.stdin.readline()

try:

segundos = int (line)

if segundos < 0 or segundos > 864000: print 'ERRO'

else:

dias = segundos / (60 * 60 * 24)

segundos -= dias * (60 * 60 * 24)

horas = segundos / (60 * 60)

segundos -= horas * (60 * 60)

minutos = segundos / 60

segundos -= minutos * 60

print (str(dias).zfill(2) + 'd' + str(horas).zfill(2) + 'h' + str(minutos).zfill(2) + 'm' + str(segundos).zfill(2) + 's')

except ValueError:

print 'ERRO'
