def interview_que(input_values):
    input_values = input_values.strip().lower()  
    greet = ['tell me about yourself']
    strength = ['what are your strengths?']
    week = ['what are your weaknesses?']
    work = ['why do you want to work here?']
    stress = ['how do you handle stress and pressure?']
    goals = ['what are your long-term career goals?']
    other = ['do you have any other questions for us?']
    
    default = "I'm sorry, I don't have a response for that question."

    if input_values in greet:
        return "I'm [Your Name]. I have [X years] of experience in [your field/industry]. I'm passionate about [mention something related to the job or industry], and I've achieved [mention any notable achievements or experiences]."

    elif input_values in strength:
        return "My strengths include [mention 2-3 relevant strengths like problem-solving, teamwork, attention to detail, etc.]. For example, I'm skilled at [mention specific skill] which has helped me [give an example of how this strength benefited you in the past]."

    elif input_values in week:
        return "One weakness I've identified is [mention a genuine weakness], but I've been working on it by [describe steps you've taken to improve]. For instance, I've been [mention what you've been doing to overcome this weakness]."

    elif input_values in work:
        return "I want to work here because I admire your company's values and I'm excited about the opportunity to contribute my skills to your team."

    elif input_values in stress:
        return "I handle stress and pressure by prioritizing tasks, staying organized, and taking short breaks when needed to stay focused and refreshed."

    elif input_values in goals:
        return "My long-term career goal is to continuously learn and grow, taking on increasing responsibilities and making meaningful contributions in my field."

    elif input_values in other:
        return "Yes, I'm curious about opportunities for growth and development within the company and how I can contribute to its success."

    else:
        return default

print("Welcome to Interview Preparation Assistance!")
while True:
    input_values = input("Question: ").lower()  

    # Exit the loop if the user enters 'exit'
    if input_values == 'exit':
        print("Exiting Interview Preparation Assistance. Goodbye!")
        break

    response = interview_que(input_values)
    print("Response:", response)

