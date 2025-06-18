import { Badge } from "@/components/ui/badge"
import { Button } from "@/components/ui/button"
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card"
import { Separator } from "@/components/ui/separator"
import { Star, GitFork, Download, ExternalLink, Code, Zap, Shield, Users, BookOpen, Heart, Github } from "lucide-react"

export default function Component() {
  return (
    <div className="max-w-4xl mx-auto p-6 space-y-8 bg-white">
      {/* Header Section */}
      <div className="text-center space-y-4">
        <div className="flex items-center justify-center gap-3">
          <div className="w-12 h-12 bg-gradient-to-br from-blue-500 to-purple-600 rounded-lg flex items-center justify-center">
            <Code className="w-6 h-6 text-white" />
          </div>
          <h1 className="text-4xl font-bold bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
            Awesome Project
          </h1>
        </div>

        <p className="text-xl text-gray-600 max-w-2xl mx-auto">
          Bu loyiha zamonaviy texnologiyalar yordamida yaratilgan ajoyib dastur. Foydalanuvchilarga qulay va samarali
          yechim taqdim etadi.
        </p>

        {/* Badges */}
        <div className="flex flex-wrap justify-center gap-2">
          <Badge variant="secondary" className="flex items-center gap-1">
            <Star className="w-3 h-3" />
            MIT License
          </Badge>
          <Badge variant="secondary" className="flex items-center gap-1">
            <GitFork className="w-3 h-3" />
            TypeScript
          </Badge>
          <Badge variant="secondary" className="flex items-center gap-1">
            <Zap className="w-3 h-3" />
            React
          </Badge>
          <Badge variant="secondary" className="flex items-center gap-1">
            <Shield className="w-3 h-3" />
            Next.js
          </Badge>
        </div>

        {/* Action Buttons */}
        <div className="flex flex-wrap justify-center gap-3">
          <Button className="flex items-center gap-2">
            <Download className="w-4 h-4" />
            O'rnatish
          </Button>
          <Button variant="outline" className="flex items-center gap-2">
            <ExternalLink className="w-4 h-4" />
            Demo ko'rish
          </Button>
          <Button variant="outline" className="flex items-center gap-2">
            <BookOpen className="w-4 h-4" />
            Hujjatlar
          </Button>
        </div>
      </div>

      <Separator />

      {/* Features Section */}
      <div className="space-y-6">
        <h2 className="text-2xl font-bold text-center">✨ Asosiy Xususiyatlar</h2>
        <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-4">
          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2 text-lg">
                <Zap className="w-5 h-5 text-yellow-500" />
                Tez va Samarali
              </CardTitle>
            </CardHeader>
            <CardContent>
              <p className="text-gray-600">Yuqori tezlik va optimal ishlash uchun optimallashtirilgan</p>
            </CardContent>
          </Card>

          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2 text-lg">
                <Shield className="w-5 h-5 text-green-500" />
                Xavfsiz
              </CardTitle>
            </CardHeader>
            <CardContent>
              <p className="text-gray-600">Zamonaviy xavfsizlik standartlari bilan himoyalangan</p>
            </CardContent>
          </Card>

          <Card>
            <CardHeader>
              <CardTitle className="flex items-center gap-2 text-lg">
                <Users className="w-5 h-5 text-blue-500" />
                Foydalanuvchi Do'st
              </CardTitle>
            </CardHeader>
            <CardContent>
              <p className="text-gray-600">Intuitiv va oson foydalaniladigan interfeys</p>
            </CardContent>
          </Card>
        </div>
      </div>

      <Separator />

      {/* Installation Section */}
      <div className="space-y-4">
        <h2 className="text-2xl font-bold">🚀 O'rnatish</h2>
        <Card>
          <CardHeader>
            <CardTitle>Tezkor Boshlash</CardTitle>
            <CardDescription>Loyihani ishga tushirish uchun quyidagi qadamlarni bajaring</CardDescription>
          </CardHeader>
          <CardContent className="space-y-4">
            <div className="bg-gray-100 p-4 rounded-lg">
              <p className="font-mono text-sm">
                <span className="text-gray-500"># Repository ni klonlash</span>
                <br />
                git clone https://github.com/username/awesome-project.git
                <br />
                <br />
                <span className="text-gray-500"># Papkaga kirish</span>
                <br />
                cd awesome-project
                <br />
                <br />
                <span className="text-gray-500"># Bog'liqliklarni o'rnatish</span>
                <br />
                npm install
                <br />
                <br />
                <span className="text-gray-500"># Loyihani ishga tushirish</span>
                <br />
                npm run dev
              </p>
            </div>
          </CardContent>
        </Card>
      </div>

      <Separator />

      {/* Usage Section */}
      <div className="space-y-4">
        <h2 className="text-2xl font-bold">📖 Foydalanish</h2>
        <Card>
          <CardContent className="pt-6">
            <div className="bg-gray-100 p-4 rounded-lg">
              <p className="font-mono text-sm">
                <span className="text-blue-600">import</span> {"{ AwesomeComponent }"}{" "}
                <span className="text-blue-600">from</span> <span className="text-green-600">'awesome-project'</span>
                <br />
                <br />
                <span className="text-blue-600">function</span> <span className="text-purple-600">App</span>() {"{"}
                <br />
                {"  "}
                <span className="text-blue-600">return</span> {"("}
                <br />
                {"    "}
                <span className="text-red-600">{"<AwesomeComponent"}</span>
                <br />
                {"      "}
                <span className="text-green-600">title</span>=<span className="text-green-600">"Salom Dunyo!"</span>
                <br />
                {"      "}
                <span className="text-green-600">theme</span>=<span className="text-green-600">"dark"</span>
                <br />
                {"    "}
                <span className="text-red-600">{"/>"}</span>
                <br />
                {"  "});
                <br />
                {"}"}
              </p>
            </div>
          </CardContent>
        </Card>
      </div>

      <Separator />

      {/* Contributing Section */}
      <div className="space-y-4">
        <h2 className="text-2xl font-bold">🤝 Hissa Qo'shish</h2>
        <Card>
          <CardContent className="pt-6 space-y-4">
            <p className="text-gray-600">Loyihaga hissa qo'shishni xohlaymiz! Quyidagi qadamlarni bajaring:</p>
            <ol className="list-decimal list-inside space-y-2 text-gray-600">
              <li>Repository ni fork qiling</li>
              <li>
                Yangi branch yarating (
                <code className="bg-gray-100 px-2 py-1 rounded">git checkout -b feature/yangi-xususiyat</code>)
              </li>
              <li>
                O'zgarishlaringizni commit qiling (
                <code className="bg-gray-100 px-2 py-1 rounded">git commit -am 'Yangi xususiyat qo\'shildi'</code>)
              </li>
              <li>
                Branch ni push qiling (
                <code className="bg-gray-100 px-2 py-1 rounded">git push origin feature/yangi-xususiyat</code>)
              </li>
              <li>Pull Request yarating</li>
            </ol>
          </CardContent>
        </Card>
      </div>

      <Separator />

      {/* Footer */}
      <div className="text-center space-y-4">
        <div className="flex justify-center items-center gap-2 text-gray-600">
          <span>Agar loyiha yoqsa, yulduzcha bering</span>
          <Star className="w-4 h-4" />
        </div>

        <div className="flex justify-center items-center gap-4 text-sm text-gray-500">
          <span className="flex items-center gap-1">
            <Heart className="w-4 h-4 text-red-500" />
            Uzbekiston bilan yaratildi
          </span>
          <span>•</span>
          <span className="flex items-center gap-1">
            <Github className="w-4 h-4" />
            MIT License
          </span>
        </div>

        <p className="text-xs text-gray-400">© 2024 Awesome Project. Barcha huquqlar himoyalangan.</p>
      </div>
    </div>
  )
}
