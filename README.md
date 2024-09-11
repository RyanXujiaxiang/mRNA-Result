Code used in the research "Mapping Global Public Perspectives on mRNA Vaccines and Therapeutics"

1. Please download the dataset from the following link: https://drive.google.com/drive/folders/12QR04mBYRZyPafsfSSYTBP07QMhMlYNY?usp=sharing

2. The following ChatGPT prompts and code were used to analyze the data in this research:

    """
   system_prompt = """
        I'm monitoring social media discussions to understand public attitudes towards the mRNA technology / vaccine. Please help me classify the provided Twitter post about the mRNA technology / vaccine.
        
        Here are the definition of safety, effectiveness, importance and trust in authority
        (1) Safety:
        - Safe: mRNA technology / vaccine is safe and reliable (with no adverse reactions, etc.)
        - Unsafe: Doubt about the safety of the mRNA technology / vaccine, or believe that the mRNA technology / vaccine is unsafe (including concerns about possible adverse reactions, or damage to health, etc.)
        (2) Effectiveness:
        - Effective: mRNA technology / vaccine is effective, to produce antibodies, or to prevent COVID-19 (or other disease), etc. (positive attitudes towards effectiveness)
        - Ineffective: Doubt about the effectiveness of the mRNA technology / vaccine, or believe that the mRNA technology / vaccine is ineffective, unable to produce antibodies or prevent COVID-19 (or other disease), etc. (negative attitudes towards of effectiveness)
        (3) Importance
        - Important: mRNA technology / vaccine is important, necessary or needed
        - Unimportant: mRNA technology / vaccine is unimportant, unnecessary or unneeded
        (4) Trust in authority
        - Trust: Trust in government or policy-makers (including all-level government, ministry of health, CDC, etc) 
        - Distrust: Doubt or distrust in government or policy-makers (including all-level government, ministry of health, CDC, etc)

        The desired output should be in JSON format:
        {
            "sentiment": "positive/neutral/negative",
            "is_misinformation": "true/false/not sure",
            "safety": "safe/unsafe/irrelevant",
            "effectiveness": "effective/ineffective/irrelevant",
            "importance": "important/unimportant/irrelevant",
            "trust": "trust/distrust/irrelevant"
        }
    """
