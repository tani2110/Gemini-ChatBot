import pathlib
import textwrap
import google.generativeai as genai
from IPython.display import Markdown
def takeCommand():
        query = input("User: ")

        return query

def to_markdown(text):
  text = text.replace('•', '  *')
  return Markdown(textwrap.indent(text, '> ', predicate=lambda _: True))

genai.configure(api_key= "") #Enter your API key

model = genai.GenerativeModel('gemini-pro')
print('Gemini is Active')

while True:

  query = takeCommand()
  response = model.generate_content(query)
  print("Gemini : ",response.text)
