# python 3.8.16
#coding utf-8

# Store the human preproinsulin sequence in a variable called preproinsulin:
preproInsulin = "malwmrllpllallalwgpdpaaafvnqhlcgshlvealylvcgergffytpktr" \
"reaedlqvgqvelgggpgagslqplalegslqkrgiveqcctsicslyqlenycn"
isInsulin = "malwmrllpllallalwgpdpaaa"
bInsulin = "fvnqhlcgshlvealylvcgergffytpkt"
aInsulin = "giveqcctsicslyqlenycn"
cInsulin = "rreaedlqvgqvelgggpgagslqplalegslqkr"

insulin = bInsulin + cInsulin
print("The sequence of insulin is: " + insulin)

print("\n--------------------------------------------------------------------\n")

#Calculating the molecular weight of insulin
# Creating a list of the amino acid (AA) weights 
aaWeights = {'A': 89.09, 'C': 121.16, 'D': 133.10, 'E': 147.13, 'F': 165.19,
'G': 75.07, 'H': 155.16, 'I': 131.17, 'K': 146.19, 'L': 131.17, 'M': 149.21,
'N': 132.12, 'P': 115.13, 'Q': 146.15, 'R': 174.20, 'S': 105.09, 'T': 119.12,
'V': 117.15, 'W': 204.23, 'Y': 181.19}  

# count the number of each amino acids in insulin
aaCountInsulin = ({x: float(insulin.upper().count(x)) for x in ['A', 'C',
'D', 'E', 'F', 'G', 'H', 'I', 'K', 'L', 'M', 'N', 'P', 'Q', 'R', 'S', 'T',
'V', 'W', 'Y']})  
print(aaCountInsulin)

# count the number of amino acid in each strain of insulin
aaCountInsulin = {}
for i in range(len(insulin)):
    if insulin[i] not in aaCountInsulin:
        aaCountInsulin[insulin[i]] = insulin.count(insulin[i])
aaCountInsulin = dict(sorted(aaCountInsulin.items()))
aaCountInsulin = {key : float(value) for key, value in aaCountInsulin.items()}
# outputs a dictionary as {aminoAcid : countOfAminoAcid}
print(aaCountInsulin)

# counts the weight of each amino acid in the insulin strain
aminoWeightInsulin = {}
for key, value in aaCountInsulin.items():
    aminoWeightInsulin[key] = value * aaWeights[key.upper()]
# outputs a dictionary as {aminoAcid : weightofAminoAcid}
print(aminoWeightInsulin)
# following code will calculate the total weight of molecular weight in insulin
sum = 0
for value in aminoWeightInsulin.values():
    sum += value
print(sum)
