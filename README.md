# 1. Представить список в обратном порядке
def reverse_list(lst):
    return lst[::-1]


# 2. Сортировка списка по убыванию абсолютного значения
def list_sort(lst):
    return sorted(lst, key=abs, reverse=True)


# 3. Поменять местами первый и последний элемент
def change(lst):
    if len(lst) >= 2:
        lst[0], lst[-1] = lst[-1], lst[0]
    return lst


# Примеры использования
nums = [3, -7, 2, -10, 5]

print("Исходный список:", nums)
print("Обратный порядок:", reverse_list(nums))
print("Сортировка по убыванию |x|:", list_sort(nums))
print("Поменяли первый и последний:", change(nums[:]))  # [:] чтобы не менять оригинал<img width="949" height="473" alt="image" src="https://github.com/user-attachments/assets/43e725d4-f844-479b-ac94-067bc57f3436" />
