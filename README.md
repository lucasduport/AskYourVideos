# Ask your videos

This project is a simple langchain project that allows users to ask questions and get answers from youtube videos.

## How it works

1. Youtube transcript is extracted from the video
2. Transcripts are splitted into chunks of 1000 characters (100 characters can overlap)
3. Each chunk is vectorized with openAI embedding API and put in a database
4. The user can query the database with a question and get the most relevant chunks
5. Langchain "stuff" to use the chunks to get the answer