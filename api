import OpenAI from "openai";

export default async function handler(req, res) {
  if (req.method !== "POST") {
    return res.status(405).json({ error: "Method not allowed" });
  }

  try {
    const { idea, genre, platform } = req.body;

    if (!idea) {
      return res.status(400).json({ error: "No idea provided" });
    }

    const client = new OpenAI({
      apiKey: process.env.OPENAI_API_KEY,
    });

    const response = await client.chat.completions.create({
      model: "gpt-4o-mini",
      messages: [{
        role: "user",
        content: `Give 5 content ideas for:
        Idea: ${idea}
        Genre: ${genre}
        Platform: ${platform}`
      }],
    });

    return res.status(200).json({
      result: response.choices[0].message.content || ""
    });

  } catch (err) {
    console.error("API ERROR:", err);

    return res.status(500).json({
      error: "Server error",
      details: err.message
    });
  }
}
