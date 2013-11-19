Exercise-2.5
============

filename = 'heathrowdata.txt'

#Data examined: first 8 lines not needed, only first 3 columns are wanted, whitspaces between elements

fp = open(filename, 'r')
raw_data = fp.readlines()
fp.close()

required_data = raw_data[7:]

data = []

for line_data in required_data:
    year_data = line_data.split()
    data.append(year_data)
    
print data[10][0]
print data[10][0:-4]

maxtemp_data = []

