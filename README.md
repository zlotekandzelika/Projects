Clinical Trial Data Analysis: Evaluating Diabetes Medication Efficacy and Safety 2025

• Conducted an end-to-end analysis of randomised controlled trial (RCT) data, investigating whether a novel diabetes medication
significantly reduced HbA1c levels compared to placebo while maintaining an acceptable safety profile.

• Managed large-scale patient-level datasets containing HbA1c measurements, demographic characteristics, medical histories, and
adverse event logs, applying data wrangling and cleaning techniques in Python (Pandas, NumPy), SQL, and Excel to remove duplicates,
impute missing values, detect outliers, and standardise categorical variables.

• Performed exploratory data analysis (EDA) to summarise baseline patient characteristics, visualise treatment effects, and identify
patterns in adverse events. Generated data visualisations such as line plots, boxplots, histograms, and bar charts in Python (Matplotlib,
Seaborn) and Power BI to communicate preliminary insights.
• Designed the study to test multiple hypotheses, including whether the treatment effect was statistically greater than placebo, whether
results varied across demographic subgroups (age, sex, ethnicity), whether disease duration influenced responsiveness, and whether
the drug maintained a favourable safety profile.
• Synthesised results into clear data-driven narratives, highlighting that the medication produced statistically significant reductions in
HbA1c, particularly among younger patients and those with shorter disease duration, while adverse events remained largely mild and
non-serious.
Thank you for your
consideration.
• Applied a range of statistical and analytical methods, including regression modelling, correlation analysis, subgroup comparisons, and
hypothesis testing, to quantify treatment effects, explore demographic interactions, and evaluate safety signals.
• Delivered a comprehensive analysis that supported regulatory approval applications, prescribing guidelines, and commercial rollout
planning, reducing uncertainty for stakeholders and strengthening the drug’s clinical and business positioning.
• Demonstrated ability to translate complex statistical findings into actionable insights, combining technical expertise with clear
communication for cross-functional teams, including regulatory, clinical, and commercial stakeholders.
• Overcame project challenges including missing data from patient dropouts and tight reporting deadlines by applying structured project
management methods, weekly stakeholder check-ins, and agile-style work planning.
• Documented analytical workflows and findings in clear, reproducible formats, ensuring that all outputs were suitable for regulatory
reporting and evidence-based decision-making.


Examples:


#for loops 
for i in range(5):
    print(i)
    
#while loops 
counter = 0
while counter <5:
    print(counter)
    counter+=1   

    person={
    "name":"bob", "age":"25", "city": "techland" 
}

#accessing values 
print(person["name"])

#modifing values 
person["age"]=26 

print(person)

def merge_sort(arr):
    if len(arr) > 1:
        mid = len(arr) // 2
        left_half = arr[:mid]
        right_half = arr[mid:]

        merge_sort(left_half)
        merge_sort(right_half)

        i = j = k = 0

        while i < len(left_half) and j < len(right_half):
            if left_half[i] < right_half[j]:
                arr[k] = left_half[i]
                i += 1

            else:
                arr[k] = right_half[j]
                j += 1
                k += 1 

                while i < len(left_half):
                    arr[k] = left_half[i]
                    i += 1
                    k += 1 

                    while j < len(right_half):
                        arr[k] = right_half[j]
                        j += 1
                        k += 1 

my_list = [64,25,12,22,11]
merge_sort(my_list)

def binary_search(arr, target):
    low, high = 0, len(arr) - 1 

    while low <= high:
        mid = (low + high) // 2 
        mid_element = arr[mid] 

        if mid_element == target: 
            return mid 
        elif mid_element < target: 
            low = mid + 1 
        else: 
            high = mid - 1 

            return -1 
            
my_list = [11,12,22,25,64]
target_element = 12 
result = binary_search(my_list, target_element)
print(f"Element {target_element} found at index {result}" if result != -1 else f"Element {target_element} not found")
    
