# multimodal-chatbot-with-image-and-pdf-support-aws
I'm elated to share a project I've been working on: a M𝘂𝗹𝘁𝗶𝗺𝗼𝗱𝗮𝗹 𝗥𝗔𝗚 based 𝗟𝗟𝗠 C𝗵𝗮𝘁𝗯𝗼𝘁 that answers questions based on 𝘂𝗽𝗹𝗼𝗮𝗱𝗲𝗱 𝗶𝗺𝗮𝗴𝗲𝘀, 𝗣𝗗𝗙𝘀 and general text queries. Isn't it great to be able to get responses based on images!

✨ 𝗞𝗲𝘆 𝗙𝗲𝗮𝘁𝘂𝗿𝗲𝘀:
𝗜𝗺𝗮𝗴𝗲 𝗮𝗻𝗱 𝗣𝗗𝗙 𝗦𝘂𝗽𝗽𝗼𝗿𝘁: Upload an image or PDF containing text, and the chatbot will extract and understand the content.
𝗧𝗲𝘅𝘁 𝗘𝘅𝘁𝗿𝗮𝗰𝘁𝗶𝗼𝗻: Utilizes OCR(Optical Character Recognition) technology to accurately extract text from images and PDFs.
General Knowledge: Capable of answering questions beyond the uploaded content.

🛠 𝗧𝗲𝗰𝗵 𝗦𝘁𝗮𝗰𝗸:
𝗘𝗮𝘀𝘆𝗢𝗖𝗥: To perform optical character recognition on uploaded images.
𝗣𝗗𝗙𝗠𝗶𝗻𝗲𝗿: For extracting text from PDF files.
𝗣𝗶𝗹𝗹𝗼𝘄 (𝗣𝗜𝗟) & NumPy: For image processing and manipulation.
𝗛𝗮𝘀𝗵𝗹𝗶𝗯: Ensures caching and efficient processing by hashing files.

𝗟𝗮𝗻𝗴𝗖𝗵𝗮𝗶𝗻:
𝗥𝗲𝘁𝗿𝗶𝗲𝘃𝗮𝗹𝗤𝗔: Constructs a question-answering system over the extracted text.
𝗣𝗿𝗼𝗺𝗽𝘁𝗧𝗲𝗺𝗽𝗹𝗮𝘁𝗲: Customizes prompts sent to the language model.
𝗙𝗔𝗜𝗦𝗦: Implements a vector store for efficient similarity search.
𝗥𝗲𝗰𝘂𝗿𝘀𝗶𝘃𝗲𝗖𝗵𝗮𝗿𝗮𝗰𝘁𝗲𝗿𝗧𝗲𝘅𝘁𝗦𝗽𝗹𝗶𝘁𝘁𝗲𝗿: Splits extracted text into manageable chunks.

𝗔𝗺𝗮𝘇𝗼𝗻 𝗕𝗲𝗱𝗿𝗼𝗰𝗸:
BedrockLLM & BedrockEmbeddings: Leverages 𝗔𝗺𝗮𝘇𝗼𝗻'𝘀 𝗧𝗶𝘁𝗮𝗻 𝗺𝗼𝗱𝗲𝗹𝘀 for language understanding and embeddings.
𝗕𝗼𝘁𝗼𝟯: AWS SDK for Python to interact with Amazon Bedrock services.

💡 𝗛𝗼𝘄 𝗜𝘁 𝗪𝗼𝗿𝗸𝘀:
𝗨𝗽𝗹𝗼𝗮𝗱 𝗣𝗵𝗮𝘀𝗲:
The app reads and processes the file, extracting text content.
𝗣𝗿𝗼𝗰𝗲𝘀𝘀𝗶𝗻𝗴 𝗣𝗵𝗮𝘀𝗲:
Extracted text is split into chunks for efficient handling.
Text chunks are converted into embeddings using Amazon's Titan embedding model.
𝗦𝘁𝗼𝗿𝗮𝗴𝗲 & 𝗥𝗲𝘁𝗿𝗶𝗲𝘃𝗮𝗹:
Embeddings are stored in a 𝗙𝗔𝗜𝗦𝗦 𝘃𝗲𝗰𝘁𝗼𝗿 𝘀𝘁𝗼𝗿𝗲.
When a question is asked, the app retrieves relevant text chunks based on similarity.
𝗔𝗻𝘀𝘄𝗲𝗿 𝗚𝗲𝗻𝗲𝗿𝗮𝘁𝗶𝗼𝗻:
The app constructs a prompt combining the context and the user's question.
𝗔𝗺𝗮𝘇𝗼𝗻'𝘀 𝗧𝗶𝘁𝗮𝗻 𝗹𝗮𝗻𝗴𝘂𝗮𝗴𝗲 𝗺𝗼𝗱𝗲𝗹 generates a concise and accurate answer.
If the context isn't sufficient, the model leverages its general knowledge.

🌟 𝗪𝗵𝗮𝘁 𝗜 𝗟𝗲𝗮𝗿𝗻𝗲𝗱:
𝗠𝘂𝗹𝘁𝗶𝗺𝗼𝗱𝗮𝗹 𝗜𝗻𝘁𝗲𝗴𝗿𝗮𝘁𝗶𝗼𝗻: Combining image and text data processing in a seamless way.
Advanced NLP techniques: Implementing retrieval-augmented generation (𝗥𝗔𝗚) to enhance answer accuracy.
AWS Bedrock Utilization: Harnessing powerful language models and embeddings from Amazon's AI services.
State Management: Efficiently managing state and caching in Streamlit to optimize performance.

🔗 Try It Out and Share Your Thoughts!
🌐 Live app: https://lnkd.in/gdgRY286
