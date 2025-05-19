# DNA-to-Text
# Define the DNA sequence
dna_sequence = "ATGCGTACATGACCGT"

# Map nucleotides to note names
note_map = {
    'A': 'C4',
    'T': 'D4',
    'G': 'E4',
    'C': 'F4'
}

print("DNA Sequence to Notes:")
print("-" * 30)

for index, base in enumerate(dna_sequence):
    note = note_map.get(base.upper(), 'Rest')
    print(f"{index + 1:>2}: {base} → {note}")
