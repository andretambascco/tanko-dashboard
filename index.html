exports.handler = async function (event) {
  const { adAccountId, accessToken, fields } = event.queryStringParameters || {};

  if (!adAccountId || !accessToken) {
    return {
      statusCode: 400,
      body: JSON.stringify({ error: "adAccountId e accessToken são obrigatórios." }),
    };
  }

  const f = fields || "id,name,currency,timezone_name,account_status,amount_spent,balance,spend_limit";
  const url = `https://graph.facebook.com/v19.0/${adAccountId}?fields=${f}&access_token=${accessToken}`;

  try {
    const res = await fetch(url);
    const data = await res.json();
    return {
      statusCode: 200,
      headers: {
        "Access-Control-Allow-Origin": "*",
        "Content-Type": "application/json",
      },
      body: JSON.stringify(data),
    };
  } catch (err) {
    return {
      statusCode: 500,
      body: JSON.stringify({ error: err.message }),
    };
  }
};
