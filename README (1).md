a = [4, 4, 5, 6, 6, 5]
f = a.group_by { |x| x }.transform_values(&:size)
max = f.values.max
puts f.select { |_, v| v == max }.keys.join(', ')
# Dz2
