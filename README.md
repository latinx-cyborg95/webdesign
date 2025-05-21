# webdesign
web design projects 
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Linkedin, Globe } from "lucide-react";

export default function Portfolio() {
  return (
    <main className="min-h-screen bg-white text-gray-900 p-6 md:p-12 font-sans">
      <section className="max-w-4xl mx-auto text-center">
        <h1 className="text-4xl font-bold mb-2">Lina Orejuela</h1>
        <p className="text-lg mb-6">
          Hey everyone, my name is Lina. I have been working as a freelance designer since 2020.
          I love turning your ideas to life and making solid brand and digital platforms.
          Here are a few examples of my work.
        </p>
        <div className="flex justify-center gap-4 mb-12">
          <a href="mailto:you@example.com" aria-label="Email">
            <Mail className="w-5 h-5" />
          </a>
          <a href="https://linkedin.com/in/yourprofile" target="_blank" aria-label="LinkedIn">
            <Linkedin className="w-5 h-5" />
          </a>
          <a href="https://yourwebsite.com" target="_blank" aria-label="Website">
            <Globe className="w-5 h-5" />
          </a>
        </div>
      </section>

      <section className="grid gap-6 md:grid-cols-3">
        <Card>
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold mb-2">Birkenhall Hommage</h2>
            <p className="text-sm mb-2">
              An independent art project and biography dedicated to a client's father.
              <br />
              <a
                href="https://dirk1616.wixsite.com/birkenhall-hommage"
                target="_blank"
                className="text-blue-600 underline"
              >
                View Project ↗
              </a>
            </p>
          </CardContent>
        </Card>

        <Card>
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold mb-2">Project Two (Placeholder)</h2>
            <p className="text-sm mb-2">
              A branding and website concept for a fictional coffee shop, demonstrating
              minimal design and strong visual storytelling.
            </p>
          </CardContent>
        </Card>

        <Card>
          <CardContent className="p-4">
            <h2 className="text-xl font-semibold mb-2">Project Three (Placeholder)</h2>
            <p className="text-sm mb-2">
              UX/UI case study for a mobile app prototype focused on event planning and community engagement.
            </p>
          </CardContent>
        </Card>
      </section>
    </main>
  );
}
